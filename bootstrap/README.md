# AquaLegend 完整源码历史归档

`bootstrap/source-history.partXX.b64` 保存 AquaLegend 2.1.1 ~ 2.5.4 的完整文本源码 Git 历史。

归档采用 Git bundle，并为每个版本创建同名 Tag：

`2.1.1, 2.2.0, 2.2.1, 2.2.2, 2.2.3, 2.3.0, 2.3.1, 2.4.0, 2.5.0, 2.5.1, 2.5.2, 2.5.3, 2.5.4`

## 还原

Linux/macOS/Git Bash：

```bash
cat bootstrap/source-history.part*.b64 | tr -d '\n' | base64 -d > AquaLegend-source-history.bundle
git clone AquaLegend-source-history.bundle AquaLegend-history
cd AquaLegend-history
git tag
git checkout 2.5.4
```

切换历史版本，例如：

```bash
git checkout 2.3.1
```

## 校验

完整 bundle SHA-256：

`d7c7128eb7de48c89691edd7b39107b0ecf6ccd8c69c335349b41d905d800da2`

归档只保存源码与文本配置/开发文档；第三方 SDK/JAR、编译产物、缓存和生成图片不作为源码重复打包。
