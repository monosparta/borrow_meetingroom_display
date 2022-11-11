# 會議室借用螢幕顯示

## 實作方法

- 使用 e-paper 串接至 ESP32，使用MicroPython。
- 架設一個樹莓派作為MQTT Broke中間站。
- 利用Python的PIL模組繪製借用的預約狀況，再將繪製好的圖片透過MQTT傳送到ESP32後，在透過ESP32傳遞至e-paper。
  - 供使用者快速看到一週內借用狀況。

## 系統需求

- ESP32
- e-paper (先列--概約尺寸，再看需求後選擇，以下2色皆為黑白)

|  尺寸  |  規格  |
|  ----  | ----  |
|  2.9"  | 有2色與3色，3色有黑白紅與黑白黃兩種版本 |
|  4.2"  | 有2色與3色(黑白紅) |
|  4.7"  | 電容式電子墨水屏觸控面板，有3色，黑白及16灰階 |
|  5.65"  | 有3色，黑白紅 |
|  5.7"  | 有7色，黑白紅綠藍黃橘 |
|  5.83"  | 有3色，黑白紅 |
|  6  | 有3色，黑白及16灰階 |
|  7.3"  | 有4色，黑白紅黃 |
|  7.5"  | 畫面分辨率有三種，640x384、800x480、880x528，有2色與3色，3色有黑白紅與黑白黃兩種版本|
|  7.8"  | 有3色，黑白及16灰階 |
|  9.7"  | 有3色，黑白及16灰階 |
|  10.3"  | 有3色，黑白及16灰階 |

## 進行方式

### 會員

- 將組裝好的螢幕顯示放置會議室門前（或門旁）
- 顯示當週會議室借用資訊

#### 管理員

- 將租借審核通過資料寫進excel（過渡）

## 預期達成目標

- 讓會員一目了然會議室一週的借用狀況
