# 1. Virtual Environment
Input the following code to create the virtual environment R2V-MIF

    conda env create -f environment.yaml

# 2. Project Directory

```
.
├── checkpoints                
│   ├── nets                   
│   ├── node_data
│   └── node_vector
├── data
│   ├── data_demo.xlsx         # Data *1 
│   └── data_tools.py
├── logs
├── args_demo.txt              # An example file.
├── dataloader.py
├── environment.yaml
├── helper.py                  # Some tools
├── main.py                    # Main entry file
├── metric.py                  # Evaluation metrics
├── models.py                  # Model : R2V-MIF
├── README_zh.md
├── README.md
└── train.py                   # Training + Testing
```


*1: data can be downloaded from the BCDB's official website: http://bcdb.mdt.team:8080

*2: Parameters serve as references (based on the data structure mentioned in the paper)."


# 3. Train and predict
Input the following code to run the project

    python main.py

# 4. Expected Running Results
## 4.1 Progress Prompt Messages
Prompts for generating/achieving rule graphs, embedding prompts for rules, information on data distribution, R2V-MIF training progress, etc.

## 4.2 Model Saving
Including three files containing the followings: the rule graph, the rules embedding, and the R2V-MIF model. They are respectively saved in the following directories: checkpoints/node_data, checkpoints/node_vector, checkpoints/nets.

## 4.3 Prediction Results
Utilizing three evaluation metrics: HR@K, MRR@K, NDCG@K, and generating prompt information during runtime.

# 5. Other Information
1. Due to privacy protection and other reasons, medical data is not uploaded. You can apply for downloading from the BCDB official website (http://bcdb.mdt.team:8080).
