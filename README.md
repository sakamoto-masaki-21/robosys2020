# ロボットシステム学　課題１
Raspberry Pi 4を用いた2つのLEDをコマンドで点滅させるデバイスドライブの作成

## 実行環境
本体：Raspberry Pi 4 Computer Model B
OS: Ubuntu 20.04

## 使用したもの
・Raspberry Pi 4

・ブレットボード

・ジャンパー線　4本

・LED　2つ

・抵抗　2つ

## 実行方法
LEDに使用したGPIOは、6番と25番である。
コンパイルの実行方法は以下のようになる。

```$ make
   $ sudo insmod myled.ko
   $ sudo chmod 666 /dev/myled0
   $ echo 0 > /dev/myled0       //LED1消滅
   $ echo 1 > /dev/myled0       //LED1点灯
   $ echo 2 > /dev/myled0       //LED2消滅
   $ echo 3 > /dev/myled0       //LED2点灯  ```

## 実行動画
<https:youtube/Q6Fmlko26hw>

## 作成者
Masaki Sakamoto and Ryuichi Ueda

## licence
GPL-3.0 License

