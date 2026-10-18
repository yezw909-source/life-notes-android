# 第三方组件与分发声明

人生随记应用源码目前不公开。本目录的许可证仅适用于对应第三方组件，**不是人生随记应用源码或品牌素材的开源许可证**。

| 组件 | 本版本依赖 | 许可证 |
| --- | --- | --- |
| Bouncy Castle | bcprov-jdk18on 1.86 | Bouncy Castle MIT-style |
| Kotlin | 2.4.20 | Apache-2.0 |
| Jetpack Compose | BOM 2026.09.00（实际 UI 1.12.1 / Material3 1.4.0） | Apache-2.0 |
| AndroidX Core / Activity / Lifecycle / Navigation | 1.18.0 / 1.13.0 / 2.11.0 / 2.10.2 | Apache-2.0 |
| Room / SQLite / DataStore | 3.0.3 / 2.7.1 / 1.2.1 | Apache-2.0；DataStore 的 shaded protobuf 为 BSD-3-Clause |
| SQLCipher for Android Community | 4.19.1 | BSD-style 3-clause；SQLite public domain；LibTomCrypt public-domain option |
| Coroutines / kotlinx.serialization | 1.11.0 / 1.11.0 | Apache-2.0 |
| OkHttp / Okio | 5.5.0 / 3.18.1 | Apache-2.0 |
| Media3 / ExifInterface | 1.11.1 / 1.4.2 | Apache-2.0 |
| Guava / JSpecify / JetBrains annotations | 33.3.1-android / 1.0.0 / 23.0.0 | Apache-2.0 |
| Native graphics math / libc++ | AndroidX/Filament-derived routines / NDK static runtime | Apache-2.0；保留 Skia 与 LLVM/legacy 相关声明 |

完整许可文本及实际 runtime 坐标见 [third-party](third-party/NOTICE.txt) 和 [清单](third-party/runtime-components.txt)。相同声明也放入 APK 的 `assets/third-party/`，供分发随附；发布时请同时提供本声明及许可证文件压缩包。测试服务器、测试框架和构建工具不是 APK runtime 组件。

许可文本来自实际依赖包及上游官方仓库；本轮未修改第三方原生源码。SQLCipher Android wrapper 与 core 分别保留原始版权年份及 BSD 条款，不能用统一 Apache 声明代替。参考：[SQLCipher Android 许可证](https://github.com/sqlcipher/sqlcipher-android/blob/v4.19.1/LICENSE)、[Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0)、[LLVM libc++ 许可证](https://github.com/llvm/llvm-project/blob/llvmorg-14.0.6/libcxx/LICENSE.TXT)。

App Icon 使用产品所有者提供并已验收的绿色时间轴素材，未重新设计；字体使用系统字体。以上归属说明不构成第三方对本产品的背书，也不代替正式发布前由产品所有者确认素材权利及服务商条款。
