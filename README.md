# GRU-PINN
This project contains a Comparison between an LSTM, GRU, and GRUPINN-based network for both SOC and SOH estimation. The choice of extending the GRU network to a Physics-informed GRU-PINN is due to the fact that the GRU outperforms the LSTM network for SOC and SOH estimation, despite having a lesser number of learnable parameters, and the aim of this project is to construct a lightweight GRU-PINN network that can potentially be deployed in a microcontroller. This was a final project for the EE598 - Deep Learning Foundations and Applications class, taught by Dr. J at Arizona State University. 

Key Findings :
1. Both the LSTM and GRU networks had similar configurations. A two layer network with 0.2 dropout. The Oxford Battery Dataset was used for all the networks.
2. The vanilla GRU network outperformed the LSTM network for both the SOC and SOH estimation.
3. The GRU-PINN network had a better understanding of the change of the SOC with respect to the cell current. 
4. The GRU-PINN network did not perform well on SOH estimation, which can be due to the fact that the feature extracted for SOH estimation had a high correlation with the SOH.
5. This can be further extended by having a more dynamic dataset. The Oxford battery dataset consisted of constant charge and discharge at different C rates.


A better understanding of the project can be found in the Project Report. 

To use the code in this repository, ensure that the dataset is located in the same directory as the code. 
