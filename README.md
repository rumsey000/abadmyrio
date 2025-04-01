# 避免雲端有時候抓不到資料而改用GitHub存放abadmyrio專案
## ServoControl_myrio

| 版本號             | 變更內容                                                   |
|------------------|-----------------------------------------------------------|
| **ServoControl_myrio_v1.vi** | - 與 **STM32控制板** 通訊，進行伺服馬達位置的輸入輸出控制。  |
| **ServoControl_myrio_v2.vi** | - 將一部分檔案包成 **subVI** 以增強模組化。<br>- **誤刪** `Myrio2RSBL.vi` 檔案，導致該版本目前不可用。 |
| **ServoControl_myrio_v3.vi** | - 將輸入輸出處理轉換為 **角度**，使控制更加精確。<br>- 新增了 **定角功能** 與 **弦波功能**。 |
| **ServoControl_myrio_v3_measure.vi** | - 新增 **CSV檔案** 輸出功能，將數據保存到本地檔案。 |
| **ServoControl_myrio_v3_FIFO.vi** | - 上一版本會導致 MyRIO 的 **RAM** 空間不足，進而中斷程式運行。<br>- 使用 **FIFO 資料結構** 來更高效地管理資料流。 |
---
## DCMotorControl

| 版本號             | 變更內容                                                   |
|------------------|-----------------------------------------------------------|
| **DCMotorControl_v0.vi** | - 控制直流馬達進行**弦波運動**<br>-原本機電課上的使用的檔案。  |
| **DCMotorControl_v1.vi** | - 控制馬達以六足步態轉動。 |
| **DCMotorControl_v1_measure.vi** | - 將輸入輸出處理轉換為 **角度**，使控制更加精確。<br>- 新增了 **定角功能** 與 **弦波功能**。 |
---
## DualMotorControl

| 版本號             | 變更內容                                                   |
|------------------|-----------------------------------------------------------|
| **DualMotorControl_v0.vi** | - 整合伺服馬達 (v3_measure) 與直流馬達 (v1_measure) 程式。  |
| **DualMotorControl_v1.vi** | - 上一版本會導致 MyRIO 的 **RAM** 空間不足，進而中斷程式運行。<br>- 使用 **FIFO 資料結構** 來更高效地管理資料流。<br> - 由於CPU仍會過載，因而將DC部分改為定PWM形式。|
| **DualMotorControl_v2.vi** | - 增加霍爾感測器量測程式(尚未完成)。 <br> - 由於CPU仍會過載，因而將DC部分改為離線傳輸六足步態目標值矩陣。(仍須測試)|

