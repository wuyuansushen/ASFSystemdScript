# ASFSystemdScript

## 1.Download ArchiSteamFarm

Download [here](https://github.com/JustArchiNET/ArchiSteamFarm/releases)

## 2.Extract downloaded package

Extract **ASF-linux-x64.zip** to Directory **/usr/bin/ArchiSteamFarm**

```
mkdir /usr/bin/ArchiSteamFarm
unzip -d /usr/bin/ArchiSteamFarm ASF-linux-x64.zip
```

> :warning: **ASF-linux-x64.zip** must be extracted in **/usr/bin** because of **SELinux**.

## 3.Enbale ArchiSteamFarm.service

```
cp ArchiSteamFarm.service /etc/systemd/system/
systemctl daemon-reload
systemctl start ArchiSteamFarm.service
```

> Tips :zany_face: : If you want to run it automatically after `reboot`, Please run `systemctl enable ArchiSteamFarm.service`
