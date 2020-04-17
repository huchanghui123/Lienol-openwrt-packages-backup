# openwrt-package

luci-app-passwall停止开发，当然如果存在BUG，欢迎各位大佬PR。

[OpenWRT-Actions](https://github.com/Lienol/openwrt-actions/actions)

请使用[基于官方openwrt源码](https://github.com/Lienol/openwrt) 和 [基于大雕源码](https://github.com/Lienol/openwrt/tree/dev-lean-lede)源码编译

使用方法：
编辑OpenWRT源码根目录 feeds.conf.default 将https://github.com/Lienol/openwrt-package 替换为 https://github.com/huchanghui123/Lienol-openwrt-packages-backup


然后执行
```bash
./scripts/feeds clean
./scripts/feeds update -a
./scripts/feeds install -a
```
或者你可以把该源码手动下载或Git Clone下载放到OpenWRT源码的Package目录里面，然后编译。
如果你使用的是Luci19，请编译时选上"luci","luci-compat","luci-lib-ipkg"后编译
