# GitHub Release v1.0.0 — 待发布说明

**待上传，尚未创建 GitHub Release。** 产品负责人已确认签名 RC1 最小真机冒烟通过并批准发布；本说明将随最终公开资产发布，不代替实际下载。

## 人生随记 1.0.0

你的私人数字生活档案。把值得留下的，留在自己手里。

首个正式分发版本，汇集记录、私人文件库、录音、提醒、随心一卦、本地加密 Vault 与加密便携备份。可自行配置 AI 服务商，在授权范围内查询文件目录、读取有限文档、追溯来源，并在单模型、并行咨询和圆桌中保留会话连续性。

本次仅正式封装既有功能，没有新增业务能力、变更数据表或备份格式。源码仍私有，公开仓库用于产品展示与版本分发。

## 待上传资产

- `LifeNotes-1.0.0-arm64.apk`：ARM64、R8 优化、非 Debuggable，沿用既有 Alpha 签名。只调整 RC1 文件名，字节和校验值不变。
- `SHA256SUMS.txt`、`SIGNING.txt`：文件校验与公开证书指纹。
- `LifeNotes-1.0.0-third-party-notices.zip`：第三方许可与分发声明；APK 内也包含对应声明。

包名 `com.localfirst.archive`；versionName `1.0.0`；versionCode `2`；最低 API 26，目标 API 37。

实际 APK：5,982,218 bytes（5.705 MiB）；SHA-256：`2bc07f70ce47966b9e846b2398eb3c67acc069fb38453f8bba6d2ae3971d4c59`。证书 SHA-256：`abb9d24eacbfd770b2b470f5178d95f8e3dc520d0c88c245056bd2ed4a9756b5`。静态签名/Debug 隔离与 16KiB ZIP/ELF 对齐检查通过；这不代替真机运行。

## 升级与隐私

旧 Alpha 同签名、旧 code < 2 才可原位升级，先主动备份；禁止通过卸载或清 Vault 解决冲突。Debug 不是可覆盖的同签名版本。安装流程见 [INSTALL](INSTALL.md)，数据与外部 AI 说明见 [PRIVACY](PRIVACY.md)。

## 必须保留的限制

产品负责人已确认签名 ARM64 RC1 的最小真机冒烟通过。真实 AI 服务、更广厂商设备、全部通知模式未完整验收；API 37 Debug 模拟器与固定 HTTPS 协议测试不能替代。大文件库滚动/授权目录查询及低内存冷启动 ANR 风险未关闭。PDF、旧 Office、扫描件与图片/音视频 AI 内容理解存在限制；后台录音和横幅提醒受系统与 OEM 设置影响。

详见 [KNOWN_LIMITATIONS](KNOWN_LIMITATIONS.md)。不公布真实凭据、私有测试日志或私人档案，不虚构用户量或远端验收成绩。

## 发布约束

公开仓库为独立的 `yezw909-source/life-notes-android`，不包含应用源码或私有开发历史。发布时核对可见性与实际资产，不将源码仓库改为 Public。后续修订必须提高 versionCode 并重新验收，不能静默替换已分发包。
