## Propose
The new approach is implemented by a freely available Python function called M-BRIT. The proposed method is implemented using the TensorFlow platform. 

## Requirement
* __document：__ requirements.txt

## M-BRITS.ipynb
In the M-BRITS.ipynb file, there are various parameters to consider. 
1."units": parameter indicates the number of elements each character is converted into. 
2."timesteps": parameter signifies the time interval between predictions and is set to 1 to prevent data reduction due to varying data lengths. 
3."learning rate ": determines how much the neural network weights are adjusted during optimization to minimize loss. 
4."batch size": refers to the number of items processed together in a batch, often set at 16, 32, or 64. 
5."epoch": parameter indicates how many times the model is trained, with higher values leading to more training but potentially slowing down processing speed. 
6."num_slices": parameter in M-BRITS represents the data interval, ranging from 2 to the end of the data, with an interval of 5 being tested in the lab experiment.

## read_result.ipynb
In the read_result.ipynb file, the parameter file_number indicates the specific iteration being performed by M-BRITS. For instance, to retrieve the results of M-BRITS(3), we should set file_number to 3. This thesis discusses two weight selection methods: PCA and AR. To generate weighted results, the weight_dict_type function must be filled with the preferred weight method.
To optimize the process, we employ the Adam optimizer starting with a learning rate of 0.001. The training is done in batches of 16 over 100 epochs, utilizing 100 units and 1 timesteps.

## Collective Result

MAE
![image](https://github.com/user-attachments/assets/fc329675-5fe6-4b7c-aa55-083897456d72)

MSE
![image](https://github.com/user-attachments/assets/d39bcd4a-dcd9-4005-8911-d9009b609d8f)

## Indivisual Result
![image](https://github.com/user-attachments/assets/8c14735c-1e9a-4c01-880c-66ee3dc54e39)
![image](https://github.com/user-attachments/assets/13ad96e9-3567-4f45-be48-7dfbd23fce4a)
![image](https://github.com/user-attachments/assets/453bf891-05dd-4c28-8185-813ac5c1c887)
![image](https://github.com/user-attachments/assets/09233740-ee17-4f95-a703-a5eb9bfb14b5)
![image](https://github.com/user-attachments/assets/dbc179b2-7777-48f1-9c59-19f10f2f56b3)






