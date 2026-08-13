# Linux 内核常见模式

## 前缀

- devm_：设备生命周期管理，自动释放
- platform_：平台设备相关
- of_：设备树相关
- clk_：时钟框架
- regmap_：寄存器抽象
- gpiod_：GPIO 描述符

## 配对

- get / put：获取/释放引用
- enable / disable：打开/关闭
- prepare / unprepare：准备/反准备
- register / unregister：注册/注销
- probe / remove：设备插入/移除
- alloc / free：分配/释放

## 返回约定

- 0：成功
- 负 errno：失败
- ERR_PTR / IS_ERR / PTR_ERR：错误指针
