
  - 

  No WSA
- How
    No way in WSA since it's mounted as read-only by Hyper-V. You can modify the system by making a Magisk module. Or directly modify the system.img. Ask Google for help.
- I cannot `adb connect localhost:58526`

    Make sure developer mode is enabled. If the issue persists, check the IP address of WSA on the setting page and try `adb connect ip:5555`.
- Magisk online module list is empty?

    Magisk actively removes the online module repository. You can install the module locally or by `adb push module.zip /data/local/tmp` and `adb shell su -c magisk --install-module /data/local/tmp/module.zip`.
- Can I use Magisk 23.0 stable or a lower version?

    No. Magisk 