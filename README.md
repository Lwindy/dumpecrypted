# dumpecrypted
本项目包含一个未签名的dumpecrypted.dylib

使用时请先查看教程：

简书：https://www.jianshu.com/p/7a173a1d7529

掘金：https://juejin.im/post/5e1a7e4ee51d455801624208

## 列出可签名证书
security find-identity -v -p codesigning

## 为dumpecrypted.dylib签名
codesign --force --verify --verbose --sign "iPhone Developer: xxx xxxx (xxxxxxxxxx)" dumpdecrypted.dylib
