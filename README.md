# android_kernel_huawei_kirin710_EMUI9.1.0_ReSukisu-Exp
拉取自：https://github.com/Coconutat/android_kernel_huawei_kirin710_KSU   
删除老旧的 KernelSU 的hook后，重新根据ReSukiSU [文档](https://resukisu.github.io/zh-Hans/guide/manual-integrate.html) 重新添加hook。  
同时根据[另一篇文档](https://kernelsu-general-porting-guide.readthedocs.io/zh-cn/latest/doc/KernelSU%E9%80%82%E9%85%8DEMUI9%E6%88%969.1.0%E7%B3%BB%E7%BB%9F%E7%9A%84%E5%86%85%E6%A0%B8.html)修改hook，修改内核配置。  
主要针对Nova5i进行适配，底包版本：EMUI9.1.0.185（C00E185R7P1），内核版本4.9.148+，SELinux为执行模式。  
## ！警告！
- 不能保证SELinux再宽容模式下开机，至少我宽容模式下无法开机（也许需要补丁）。  
开机后可以手动设置宽容，这没问题。
- 未验证：只保证生成的内核二进制文件：out/arch/arm64/boot/Image 可以正常开机，内核目录下生成的镜像不保证其可用性。
