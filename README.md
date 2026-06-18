# 8800Pro Android

森海克斯 8800Pro 写频工具的 Android 客户端，代码独立于网页端和 iOS 端维护。

## 功能

- 蓝牙连接、读频、写频和全局进度提示
- 信道区域切换、区域名称编辑、信道新增、复制、剪切、粘贴、插入和删除上移
- 信道频率、亚音、功率、带宽、扫描加入、忙锁和 PTT ID 编辑
- HamCQ 中继台库，支持按大区、省份和关键词筛选后写入当前信道
- VFO、DTMF、FM 收音机、本地快照、恢复和通信日志
- 空信道安全写入、原始数据块保留、区域名称和中文信道名 GBK 编解码

## 仓库关系

- 网页端：`BG7OWW/8800Pro-Web`
- iOS 端：`BG7OWW/8800Pro-iOS`
- Android 端：当前仓库

三个平台分仓维护，避免网页仓库携带移动端工程体积，也方便各平台独立发布。

## 本地构建

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk --release
```

如果需要正式发布签名，请在 `android/key.properties` 中配置本地 keystore。私钥文件不要提交到 GitHub。
