# DS340w Project - Automatic Stock Trading

- This is a project repository for DS340w course. 
- The project is focusing on stock price prediction. 

- The project is highly influenced by the previous research - Deep Reinforcement Learning for Automated Stock Trading: An Ensemble Strategy (https://github.com/AI4Finance-Foundation/FinRL/blob/master/tutorials/2-Advance/FinRL_Ensemble_StockTrading_ICAIF_2020.ipynb)

- The name scheme of each jupyter notebook is: 

  *** TrainingStartYear_Novelty_VersionOrdinal ***  (versionOrdinal means the order we created each version of models)
  - several different novelty
    - 6indicators --- adding 2 additional tech indicators (features) to the original model (4 tech indicators already included in the origibal model)
    - 5Agents --- 5 Agents ensembled (PPO, A2C, SAC, TD3, DDPG)
    - Valid --- change of validation ratio
    - NULL --- no novelty
    - NewAgent --- replace one of the orginal agents that was ensmbled in parent paper

- The structure of this repository:
  - 'ParentPaper.pdf' ----- pdf of parent paper
  - 'Original_2009_ParentPaper.ipynb' ----- implementation of original parent paper (data cover upto 2021-07-06)
    - Sharpe Ratio 1.96 
  - 'Original_2009_Updated_ParentPaper.ipynb' ----- updated implementation of original parent paper (data cover upto 2022-03-21)
    - Sharpe Ratio -0.14 
  - 'FinalModel_2006_NULL_version3_2.ipynb' ----- The final version of modified implementation -
    - Sharpe Ratio 0.94
  - 'FunVersion_2006_NULL_version3_2.ipynb' ----- The final version of modified implementation with our chosen stocks
    - Sharpe Ratio 0.64

  - SingleAgentModel ----- Folders of 5 single agent model
    - '2006_A2C.ipynb' ----- Sharpe Ratio 0.57
    - '2006_PPO.ipynb' ----- Sharpe Ratio 0.58
    - '2006_SAC.ipynb' ----- Sharpe Ratio 0.16
    - '2006_TD3.ipynb' ----- Sharpe Ratio 0.58
    - '2006_ddpg.ipynb' ----- Sharpe Ratio 0.44

  - FinRL-Library ----- Folders of FinRL library, which is created by the authors of parent paper
    - 2 modification made by us under (finrl --- drl_agents --- stablebaselines3)
      - 'models.py' --- original ensemble method created by authors of the library (A2C, PPO, and ddpg)
      - 'models_modified.py' --- ensemble A2C, PPO, and TD3
      - 'models_modified2.py' --- ensemble A2C, PPO, SAC, TD3, and ddpg

  - 2009Model ----- data start traing year in 2009
    - '2009_6indicators_version2.ipynb' ----- Sharpe Ratio 0.86

  - 2006Model ----- data start traing year in 2006
    - '2006_5Agents_version8_3.ipynb' ----- Sharpe Ratio 0.36
    - '2006_6indicators_version3.ipynb' ----- Sharpe Ratio 0.57

  - 1998Model ----- data start traing year in 1998
    - '1998_6indicators_version4.ipynb' ----- Sharpe Ratio 0.51
    - '1998_NULL_version5.ipynb' ----- Sharpe Ratio 0.97
    - '1998_NewAgent_version6.ipynb ' ----- Sharpe Ratio 0.56
    - '1998_Valid_version5_2.ipynb' ----- Sharpe Ratio 0.81

  - 1997Model ----- data start traing year in 1997
    - '1997_5Agents_version8_2.ipynb' ----- Sharpe Ratio 0.57

  - 1962Model ----- data start traing year in 1962
    - '1962_5Agents_version8.ipynb' ----- Sharpe Ratio 0.19
    - '1962_6Indicators_version7.ipynb' ----- Sharpe Ratio 0.20
