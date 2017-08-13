# CSDN 2017.8.14 《深入探讨Linux/VxWorks设备树》的案例
包含一个dtsi和一个dts。
dtsi是对于linuxer,demosoc的描述；
dts是针对上述芯片的一个evb board。

## 直播和录播地址：
http://edu.csdn.net/huiyiCourse/detail/465

## ppt下载：
https://mp.weixin.qq.com/s?__biz=MzAwMDUwNDgxOA==&mid=2652662087&idx=1&sn=c7e192f20cd1d2797fde795986312a62&chksm=810f2fdab678a6ccbaa779004ce684d296167cda125f4397667ba2a42cc408fb7de789716a24#rd

## 在该目录编译dts：
dtc -I dts -O dtb linuxer-demosoc-evb.dts -o linuxer-demosoc-evb.dtb
## 反编译：
dtc -I dtb -O dts linuxer-demosoc-evb.dtb -o 1.dts
或者
fdtdump linuxer-demosoc-evb.dtb > 1.dts

1.dts就是从dtb反编译到dts的结果。



