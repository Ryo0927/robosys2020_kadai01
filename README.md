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
### 回路


### demo
https://youtu.be/wLo6FI101Yo
