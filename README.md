# Multigroup-Neutron-Diffusion-Equation-Solver
本程序为简易的多群中子扩散方程求解程序，为核反应堆物理课程实践。

参考了《核反应堆物理分析》（谢仲生）第5版第5章5.3节 多群扩散方程的数值求解。

有待后续改进之处：
- 初始参数设置
- `update_phi`函数中`dx`和`dy`网格设置为非均匀，相应更新`k_eff`时做积分处理
- 根据收敛判断1和5调整初始值使得`k_eff`接近于1
- 函数封装
- numpy改为tensor，使用cuda加速


