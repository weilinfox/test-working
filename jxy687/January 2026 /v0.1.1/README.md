# 针对RuyiSDK Eclipse插件的测试

## 测试说明

以手动测试的方法，测试 [ruyisdk-eclipse-plugin](https://github.com/ruyisdk/ruyisdk-eclipse-plugins/commit/3e669ebb3961b948a4dd242fe9a404ad7bb1306f)

## 安装方法

- 见 [ruyisdk-eclipse-plugins/releases](https://github.com/ruyisdk/ruyisdk-eclipse-plugins/releases)

## 环境配置

+ OS: Ubuntu 24.04.3
+ Eclipse 版本
    - Eclipse IDE for C/C++ Developers (includes Incubating components)
    - Version: 2025-12 (4.38.0)
    - Build id: 20251204-0850

## 测试结果

共 12 个测试用例，成功 9 个，失败 3 个。
|          测试用例          | 结果  |                                          备注                                          |
| :------------------------: | :----: | :----------------------------------------------------------------------------------------------------------: |
|  RuyiSDK管理/自动检测与安装 ruyi | 失败  |  下载 ruyi 过程中部分按钮未 disable                                |
|  新闻/切换仅未读 | 成功  |  在白色主题下，Unread Only 勾选不明显                                |
|  虚拟环境/创建虚拟环境并应用到项目 | 失败  |  虚拟环境不在项目目录无法检测，profile 列表排序不一致                     |
|  虚拟环境/虚拟环境删除后项目目录更新 | 失败  |  无法自动更新，只能手动                     |

