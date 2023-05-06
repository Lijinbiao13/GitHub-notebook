# GitHub-notebook
## stable-baselines3学习笔记
1.显示学习进度条
```
model.learn(total_timesteps=int(2e5), progress_bar=True)
# progress_bar=True表示显示学习进度条
```
2.矢量化环境的创建
```
num_cpu = 4
vec_env = make_vec_env(env_id, n_envs=num_cpu, seed=0, vec_env_cls=SubprocVecEnv)
```
