如果在已root的安卓设备上错误操作openeuicc，导致变成单卡手机，第二卡槽消失，可以使用以下方法恢复。

Dual SIM Dual Standby (DSDS) is a handy feature for managing two SIM cards on Android devices. Accidentally disabling it using hidden codes like ##4636## can be frustrating, but on rooted devices, there's a way to restore it in three simple steps:

1 - Get Terminal Emulator: Open cmd with Run As Administrator.

2 - Enter Command: Input the command:

* adb shell uname -a

* adb shell su -c "setprop persist.vendor.radio.multisim_switch_support true"

* adb shell su -c "setprop persist.radio.multisim.config dsds"

* then Reboot your phone.

If point 2 of step 2 says permission denied, then you need to grant root permission as I was using Magisk.

Remember, rooting your device has risks, so proceed cautiously. This solution may not work for all devices, and it's wise to back up your data before attempting any changes.
