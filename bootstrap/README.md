# AquaLegend 完整源码历史归档

本仓库归档 AquaLegend 从 2.1.1 到 2.5.5 的完整源码历史。

历史归档采用 Git bundle，并为每个版本创建同名 Tag：

`2.1.1, 2.2.0, 2.2.1, 2.2.2, 2.2.3, 2.3.0, 2.3.1, 2.4.0, 2.5.0, 2.5.1, 2.5.2, 2.5.3, 2.5.4, 2.5.5`

完成导入后可从：

`bootstrap/AquaLegend-source-history-2.1.1-to-2.5.5.bundle`

还原完整 Git 历史。

## 还原

```bash
git clone bootstrap/AquaLegend-source-history-2.1.1-to-2.5.5.bundle AquaLegend-history
cd AquaLegend-history
git tag
git checkout 2.5.5
```

切换历史版本，例如：

```bash
git checkout 2.3.1
```

完整 bundle SHA-256：

`67bb1497512e6d7a68a4dabb57f257b314cd2c557bbb5702d7accf98f017d864`

归档只保存源码与文本配置/开发文档；第三方 SDK/JAR、编译产物、缓存和生成图片不作为源码重复打包。
