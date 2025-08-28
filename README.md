## 项目简介

NFC Bridge是一个创新的Android应用系统,实现了银行卡信息的无线读取、传输与模拟功能。该系统由两个主要组件构成:读卡端和模拟端,通过网络连接实现数据的安全传输。


![1747642761048](https://github.com/user-attachments/assets/012d138a-6033-430e-b157-b50ec69026ae)

![IMG_8541](https://github.com/user-attachments/assets/d8b90670-2d28-4468-8cc6-72e0287f4474)

## 核心功能

- **银行卡信息读取**:通过NFC技术读取EMV兼容的银行卡信息
- **数据安全传输**:使用Socket通信在设备间安全传输卡片数据
- **EMV卡片模拟**:利用Host Card Emulation(HCE)技术实现EMV规范下的卡片模拟
- **与POS机交互**:支持完整的EMV交易流程,包括应用选择、数据读取和交易处理
- **跨设备操作**:支持在两台设备间工作,实现卡片信息的远程使用

## 技术架构

- Android NFC API
- EMV协议实现
- Host Card Emulation(HCE)
- Socket网络通信
- APDU指令处理

## 系统要求

- Android 5.0 (API级别21)或更高版本
- 支持NFC功能的设备
- 网络连接(Wi-Fi或移动数据)

## 安装说明

1. 从Release页面下载最新APK文件
2. 在Android设备上安装应用
3. 确保设备已启用NFC功能
4. 按照应用内指南设置读卡端和模拟端

## 使用指南

### 读卡端设置
1. 打开应用并选择"读卡模式"
2. 配置网络连接参数
3. 将银行卡靠近设备背面进行读取
4. 确认读取成功后,数据将自动传输到模拟端

### 模拟端设置
1. 打开应用并选择"模拟模式"
2. 配置接收连接参数
3. 等待接收来自读卡端的数据
4. 数据接收成功后,将设备背面靠近POS机进行交易

## 项目结构

```
nfcbridge/
├── app/                    # 应用主模块
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/       # Java源代码
│   │   │   │   ├── reader/ # 读卡功能实现
│   │   │   │   ├── emulator/ # 模拟功能实现
│   │   │   │   ├── network/ # 网络通信实现
│   │   │   │   └── utils/  # 工具类
│   │   │   ├── res/        # 资源文件
│   │   │   └── AndroidManifest.xml
│   │   └── test/           # 单元测试
├── emvlib/                 # EMV协议实现库
└── nfclib/                 # NFC操作封装库
```

## 安全说明

**注意**: 本项目仅用于技术研究和学习目的。请勿用于任何未经授权的金融交易或可能违反法律法规的活动。用户需自行承担使用本应用的所有风险和责任。


## 联系方式

如有任何问题或建议,请通过Issue或以下方式联系我,请注明来意:

- Email: [weitengfei0212@gmail.com]
- ✈️ :<img width="784" height="828" alt="wechat_2025-08-28_155843_282" src="https://github.com/user-attachments/assets/6601dc6f-c9ee-42bb-bc58-2e3d8a9906cd" />
- Wechat:

