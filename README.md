# dumpecrypted
本项目包含一个未签名的dumpecrypted.dylib

使用时请先查看教程()。

# 列出可签名证书
security find-identity -v -p codesigning

# 为dumpecrypted.dylib签名
codesign --force --verify --verbose --sign "iPhone Developer: xxx xxxx (xxxxxxxxxx)" dumpdecrypted.dylib
