# 為避免雲端有時候抓不到資料而改用GitHub測試
## myRIO
### ServoControl_myrio_v1.vi
- 與stm32控制板通訊輸入輸出伺服馬達位置
### ServoControl_myrio_v2.vi
- 將一部分檔案包成subvi 
- 由於誤刪 Myrio2RSBL.vi 因此目前不可用
### ServoControl_myrio_v3.vi
- 將輸入輸出處理成角度
- 新增定角與弦波功能
### ServoControl_myrio_v3_measure.vi
- 新增將資料寫入csv檔案功能
### DCMotorControl_v0.vi
- 控制直流馬達進行弦波運動
- 原本機電課上的使用的檔案
### DCMotorControl_v1.vi
- 控制馬達以六足步態轉動
### DCMotorControl_v1_measure.vi
- 新增將資料寫入csv檔案功能
### DualMotorControl_v0.vi
- 整合伺服馬達 (ServoControl_myrio_v3_measure.vi) 與直流馬達 (DCMotorControl_v1_measure.vi) 程式
## Computer 
### servo_motor_drive_computer.vi
- 為了測試目標速度圖中等速段有突降的現象而測試用的檔案