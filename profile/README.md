# Hi there 👋

We are KarKit GoGoGo!
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
## 这里是DES3802 交互设计1

🙋‍♀️ 上海交通大学设计学院2020级工业设计专业必修课：交互设计一第四小组大作业代码部分

🍿 本小组意在于为驾驶环境的简单测试开发工具包

🧙 我们的成员有：wujinhjun/EvaLiuYW/xqxuan/...等六人

***

## 技术组成

### 硬件端

#### [Arduino](https://github.com/KarKit-Go/Arduino_for_car)

* 作用：小车的驱动体系核心，搭载了为小车构建的有限状态机
* 选型原因：流通的大部分电机驱动拓展板都是为Arduino打造的，加之本人对arduino更熟练些，遂选用
* 代码：
  * [硬串口控制](https://github.com/KarKit-Go/Arduino_for_car/tree/main/arduino/Serial_Car/)
  * [软串口控制](https://github.com/KarKit-Go/Arduino_for_car/tree/main/arduino/Serial_Car_Softserial/)

#### [ESP32](https://github.com/KarKit-Go/ESP_32_server)

* 作用：信息传递，用于服务器与小车间的信息传递
* 选型原因：搭载wifi与蓝牙，更利于无线通讯
* 代码：
  * [microWebServer](https://github.com/KarKit-Go/ESP_32_server/tree/main/ESP32/server/)
  * [wifi配置](https://github.com/KarKit-Go/ESP_32_server/tree/main/ESP32/config_wifi/)
  * [wifi配网](https://github.com/KarKit-Go/ESP_32_server/tree/main/ESP32//newBoard/)

### 软件端

#### 手机端

* 作用：通过陀螺仪判断手机的姿态，控制小车的方向
* 选型原因：容易获得，且传感器精度高，自带网络、浏览器等基础设施
* 代码：
  * [手机端web（试验用无样式）](https://github.com/KarKit-Go/DES3802_interactionDesign/tree/main/Device/)

#### mixly封装
