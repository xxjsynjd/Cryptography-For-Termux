# Cryptography For Termux (Python 3.14)

Termux 上直接 `pip install cryptography` 会报 `cannot locate symbol "PyLong_Type"`。
本仓库通过源码强制编译（禁用 abi3，生成 cp314 专属包），解决了符号隐藏导致的崩溃问题，并附带了编译好的 aarch64 wheel 包。

## 使用方法
直接安装本目录下的 wheel：
```bash
pip install cryptography-*-android_24_arm64_v8a.whl
```

