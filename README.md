# RL
Ideas
可以做一个multi Agent RL和 RL的对比
## 具体的实现步骤
### 环境的搭建
1. Create Grid World Environment
初始条件设置为[3,4],也就是3行4列共12个方格。12个方格中，有6个是可以移动的，同时边界条件是这六个方格的位置加上原来的边界
2. Create Q learning agent 
定义learning rate 和 epsilon
3. Train Q-Learning Agent
什么时候停止训练-->连续十几次得到最优解or二十次中有十五次得到最优解or三十次中有十次得到最优解or次优解也可以接受
