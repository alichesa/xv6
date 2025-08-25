# 硬件
- 半双工是发送器与接收器之间只有一根总线相连接，而全双工是两条总线相连接

- URAT通信协议的中文名称通常为 ​​“通用异步收发传输器”​​（Universal Asynchronous Receiver/Transmitter）。起始-数据-校验-结束
<img width="697" height="250" alt="image" src="https://github.com/user-attachments/assets/42bb30a4-d993-4185-b1f7-f88e2cdcf037" />

- 波特率来进行区分，比如波特率为1，每秒发送1位，那么接收方一秒接收到‘0’，发送的就是01；如果两秒接收到‘0’，那么发送的就是0011

- I2C 使用两条线在主控制器和从机之间进行数据通信，I2C 是支持多从机的，也就是一个 I2C 控制器下可以挂多个 I2C 从设备
<img width="861" height="311" alt="image" src="https://github.com/user-attachments/assets/f17a419d-d770-4af9-85b5-f734d9488135" />

- I2C起始位 -- 时钟为高，数据为低  I2C停止位 -- 时钟和数据都是高

- I2C 总线在数据传输的时候要保证在 SCL 高电平期间， SDA 上的数据稳定，因此 SDA 上的数据变化只能在 SCL 低电平期间发生
<img width="951" height="282" alt="image" src="https://github.com/user-attachments/assets/4a8af527-7422-4f21-9e22-9280b5c2583d" />

<img width="956" height="344" alt="image" src="https://github.com/user-attachments/assets/e48e6e80-9177-47b0-aa7f-fc7079c32fc3" />
​​SPI​​：高速、全双工，适合 Flash、ADC 等，但硬件复杂。
​​UART​​：简单、点对点，适合调试，但需固定波特率，仅支持异步通信
USART：不仅支持同步还支持异步，有时钟信号，不需要波特率
​​I2C​​：多设备共享、中等速度，适合传感器，但需上拉电阻。



