<div align = center>

<img src="./.assets/DogDayAndroid.png" width="200" height="175" alt="banner">

<h1>小米骁龙845系列构建KernelSU</h1>

![License](https://img.shields.io/static/v1?label=License&message=BY-NC-SA&logo=creativecommons&color=green)
![Language](https://img.shields.io/github/languages/top/Xiaomi-sdm845-KSU/Android-Kernel-Builder)
![Issues](https://img.shields.io/github/issues/Xiaomi-sdm845-KSU/Android-Kernel-Builder)
![Pull Requests](https://img.shields.io/github/issues-pr/Xiaomi-sdm845-KSU/Android-Kernel-Builder)
<br>

这个GitHub Action包含了官方内核和ngk内核

使用normal运行一次得到最新稳定版的KernelSU，使用main运行一次得到最新开发版的KernelSU

*注：[KernelSU 1.0 及更高版本已经不再支持非 GKI 内核](https://github.com/tiann/KernelSU/issues/1705)，使用此 Action 编译的内核 KernelSU 版本均为 **v0.9.5***

*注 2：由于KernelSU 1.0 及更高版本不再支持非 GKI 内核，`main` 与 `normal` 运行后的结果及产物相同，故已**移除** `main` 相关的 workflows，仅保留 `normal`*


包含: MI 8, MIX2S, POCOPHONE F1, MI 8UD, MIX 3, MI 8 Explorer Edition

*2025.2.9注：已更新workflow，使其~~应该~~能够正常运行*
<br>
</div>

---


# 内核选择


MIUI ROM 建议选择 机型代号-Xiaomi_Kernel_OpenSource-sdm845_构建时间.zip

如: 小米 MIX3 MIUI 12.5.1 选择 perseus-Xiaomi_Kernel_OpenSource-sdm845_********.zip

类原生ROM 建议选择 机型代号-NGK_android_kernel_xiaomi_sdm845_构建时间.zip

如: 小米 MIX3 类原生ROM 选择 perseus-NGK_android_kernel_xiaomi_sdm845_********.zip

MIX3使用TWRP刷入报错请使用手动修补


---


# 使用方法


Fork 本仓库后在 Actions 页面选择选择适合您的 workflow，之后点击右侧的 `Run workflow` 按钮运行编译

若编译成功，可前往 Release 页面下载对应的 zip ，在 TWRP 等 Recovery 下刷入即可

---


# 致谢


- [Akitlove](https://github.com/Akitlove) : 此项目所用99%+代码来自此作者,包括但不限于内核修复、Github Action
- [KernelSU](https://github.com/tiann/KernelSU) : KernelSU

# 许可

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">知识共享署名-非商业性使用-相同方式共享 4.0 国际许可协议</a>进行许可。
