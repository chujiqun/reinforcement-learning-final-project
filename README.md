# reinforcement-learning-final-project
强化学习期末大作业

程序代码由[Starter Kit - NeurIPS 2020 Flatland Challenge](https://gitlab.aicrowd.com/flatland/flatland-starter-kit) 修改得来

环境的配置及测试代码运行方式参见[Make a submission](https://flatland.aicrowd.com/getting-started/first-submission.html)

-------------
our_observation训练


```bash
python reinforcement_learning/model_test.py
```

实验中调节的arguments：
```python
  -n 训练epoch数
  -t 训练环境选择
  -e 测试环境选择
  --hidden_size fc层的参数
  --last_checkpoint 从某个模型继续训练
  --observation_num our_observation使用的node数
  --max_depth 树搜索的最大深度
 ```
 例如训练md=3，s=8的模型，训练环境选择test0，则命令如下:
 
 ```bash
 python reinforcement_learning/model_test.py -n 1500 -t 0 -e 0 --observation_num 8 --max_depth 3
 ```
