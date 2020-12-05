# robosys_kadai01

### 概要
LED緑1個,黄1個と抵抗2個を使い,入力によってそれぞれのLEDが光り消える,かつ2つのLEDが交互に光る.

### 動作環境
- Rasberry Pi Model 3B+
- Ubuntu18.04

### 動作
```
$echo 0 > /dev/myled0
緑のLEDが光る
$echo 1 > /dev/myled0       
緑のLEDが消える
$echo 2 > /dev/myled0       
黄のLEDが光る
$echo 3 > /dev/myled0       
黄色のLEDが消える
$echo 4 > /dev/myled0       
2つのLEDが交互に光る
```
### 実行する手順
```
$git clone https://github.com/yukikimuramura/robosys2020_kadai01.git
$cd robosys2020_kadai01
$make
$sudo insmod myled.ko
$sudo chmod 666 /dev/myled0
$echo [光らせたい動作の番号] /dev/myled0
$sudo rmmod myled
```
### 回路図
緑のLEDをGPIO25につなげ,黄色のLEDをGPIO26につなげました.
![kairo](https://user-images.githubusercontent.com/54853881/101240727-74108980-3734-11eb-8ad7-f8c7e62d0a45.png)

### demo
こちらが実際に動かした動画のURLです.
https://youtu.be/wLo6FI101Yo
