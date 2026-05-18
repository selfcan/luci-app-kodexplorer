# luci-app-kodexplorer

基于前人成果修改，完美适配 **PHP8** 并添加了 **HTTPS 支持**。在官方 OpenWrt 25.12 固件下编译测试通过，可正常使用。

---

## 🛠️ 使用方法

### 1. 克隆源码到本地

在您的 OpenWrt 编译根目录下执行以下命令，将插件下载到 `package` 目录中：

```bash
git clone https://github.com/OldCoding/luci-app-kodexplorer package/luci-app-kodexplorer
```

### 2. 在菜单中选中该插件

执行 `make menuconfig` 进入配置菜单，依次选择并勾选：

LuCI -> 3. Applications -> luci-app-kodexplorer

### 3. 依赖配置说明

🔹 OpenWrt / ImmortalWrt 源码环境
请务必开启以下功能：

    Languages ---> PHP8 ---> php8

    					---> Configuration  --->Enable LIBXML support

    										--->Enable DOM support

    										--->Enable gettext support

    										--->Enable Internationalization support

    										--->Use system timezone data instead of PHP's built-in database

🔹 LEDE 源码环境
请开启以下功能：

	Languages ---> PHP8 ---> php8
