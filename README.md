## Xiaomi SM8350 Device DrfccvKernel ##

## 支持设备 ##
- Xiaomi 11 (venus)
- Xiaomi 11 Pro (mars)
- Xiaomi 11 Ultra (star)

## 内核特性 ##
- 版本：5.4.302
- ReSukiSU v4.2.0-rc1 + SuSFS v2.1.0

## 需要注意 ##
- 基于 AlphaDroid Android 16
- 仅在小米11（venus）上经测试通过

## 工具配置 ##
- Clang 18.1.3 & LLD 18.1.3

## 开始编译 ##
```sh
make -j"$(nproc)" ARCH=arm64 LLVM=1 LLVM_IAS=1 O=out \
     TARGET_PRODUCT=venus CONFIG_DISPLAY_BUILD=y Image
```

## 引用 ##
- https://github.com/AlphaDroid-devices/kernel_xiaomi_lisa
- https://github.com/kamikaonashi/kernel_xiaomi_sm8350
- https://github.com/Baka-SU/BakaSU
- https://github.com/simonpunk/susfs4ksu
