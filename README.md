# 跨Region AutoScalingGroup解决方案

当一个region的spot实例不足导致无法启动spot EC2实例时，启动临近region的EC2 spot实例，从而达到最佳性价比。本文假设使用region为Virginia，利用AWS跨region是骨干网的特性，在Virginia不能启动G4dn.xlarge实例时，从Ohio启动G4dn.xlarge实例。

## 架构图
