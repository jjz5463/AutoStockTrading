# DS340w Project - Automatic Stock Trading

- This is a project repository for DS340w course. 
- The project is focusing on stock price prediction. 

- The project is highly influenced by the previous research - Deep Reinforcement Learning for Automated Stock Trading: An Ensemble Strategy (https://github.com/AI4Finance-Foundation/FinRL/blob/master/tutorials/2-Advance/FinRL_Ensemble_StockTrading_ICAIF_2020.ipynb)

- The name scheme of each jupyter notebook is: 

  *** TrainingStartYear_Novelty_VersionOrdinal ***
  
  (versionOrdinal means the order we created each version of models)

- The structure of this repository:
  - 'ParentPaper.pdf' ----- pdf of parent paper
  - 'Original_2009_ParentPaper.ipynb' ----- implementation of original parent paper (data cover upto 2021-07-06)
  - 'Original_2009_Updated_ParentPaper.ipynb' ----- updated implementation of original parent paper (data cover upto 2022-03-21)
  - 'FinalModel_2006_NULL_version3_2.ipynb' ----- The final version of modified implementation
  - 'FunVersion_2006_NULL_version3_2.ipynb' ----- The final version of modified implementation with our chosen stocks
  - SingleAgentModel ----- Folders of 5 single agent model
    - '2006_A2C.ipynb' ----- Sharpe Ratio 0.57
    - '2006_PPO.ipynb' ----- Sharpe Ratio 0.58
    - '2006_SAC.ipynb' ----- Sharpe Ratio 0.16
    - '2006_TD3.ipynb' ----- Sharpe Ratio 0.58
    - '2006_ddpg.ipynb' ----- Sharpe Ratio 0.44
