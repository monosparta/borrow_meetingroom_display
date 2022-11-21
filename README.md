# 會議室借用螢幕顯示

## 實作方法

- 使用 e-paper 串接至 [ESP32](https://www.waveshare.com/wiki/E-Paper_ESP32_Driver_Board#Local_Demo)，語法使用MicroPython。
- 架設一個樹莓派作為MQTT Broke中間站。
- 透過API取得當天租借的資料
- 利用Python的PIL模組繪製借用的預約清單，並將繪製好的圖片透過MQTT傳送到ESP32後，再透過ESP32傳遞至e-paper。
  - 供使用者快速看到一天內借用狀況。

## 系統需求

- ESP32
- Ｗaveshare e-paper (會以7.5“為主)

|  型號  |  分辨率  |  顯示顏色  |
|  ----  | ---- | ---- |
|  4.2inch e-Paper Module  | 400×300 | 有2色款（黑、白）與3色款（黑、白、紅，代號（B））（黑、白、黃，代號（C）） |
|  4.37inch e-Paper Module (G)  | 512×368 | 4色款（红、黄、黑、白） |
|  5.65inch e-Paper Module (F)  | 600×448 |有7色款，黑白紅黃藍綠橘 |
|  5.83inch e-Paper HAT  | 648×480 |有2色款（黑、白）與3色款（黑、白、紅，代號（B）） |
|  7.3inch e-Paper HAT (G)  | 800 × 480 |4色款（红、黄、黑、白） |
|  7.5inch e-Paper HAT  | 640x384（V1）、800×480（V2） | 有2色款（黑、白）與3色款（黑、白、紅，代號（B）） |

## 進行方式

- 將組裝好的螢幕顯示放置會議室門前（或門旁）
- 顯示當天會議室借用資訊

## 預期達成目標

- 讓會員靠近會議室時一目了然會議室一天的借用狀況
