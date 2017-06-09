# Fairphone 2 CM14.1 port

- End user thread: https://forum.fairphone.com/t/using-lineageos-on-the-fp2/28848
- Development thread: https://forum.fairphone.com/t/porting-lineageos-to-fp2/27530

# Continous Integration

- Jenkins instance: https://fp2.joutubes.nl/jenkins/
- Latest build results: https://fp2.joutubes.nl/builds/full/

# Repo config

`.repo/local_manifests/fp2.xml`
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
    <remote fetch="https://github.com/" name="github2" />
    <project name="WeAreFairphone/android_device_fairphone_FP2" path="device/fairphone/FP2" remote="github2" revision="cm-14.1" />
    <project name="WeAreFairphone/android_kernel_fairphone_msm8974" path="kernel/fairphone/msm8974" remote="github2" revision="cm-14.1" />
    <project name="WeAreFairphone/proprietary_vendor_fairphone" path="vendor/fairphone/FP2" remote="github2" revision="cm-14.1" />
    <project name="lineageos/android_device_qcom_common" path="device/qcom/common" remote="github2" revision="cm-14.1" />
</manifest>
```


# Device configuration for Fairphone 2

## Spec Sheet

| Feature                 | Specification                     |
| :---------------------- | :-------------------------------- |
| CPU                     | Quad-core 2.26 GHz Krait 400      |
| Chipset                 | Qualcomm MSM8974AB Snapdragon 801 |
| GPU                     | Adreno 330                        |
| Memory                  | 2GB RAM LPDDR3                    |
| Shipped Android Version | 5.1                               |
| Storage                 | 32GB eMMC5                        |
| MicroSD                 | Up to 128GB                       |
| Battery                 | 2420 mAh at 3.8V (9.2 Wh)         |
| Dimensions              | 143 x 73 x 11 mm                  |
| Display                 | 1080 x 1920 pixels, LCD TFT/IPS   |
| Camera                  | 8MP CMOS, Omnivision OV8865       |
| Release Date            | December 2015                     |
