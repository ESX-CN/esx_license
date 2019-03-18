# esx_license
老弟办证吗？

## 下载 & 安装

### 使用 Git
```
cd resources
git clone https://github.com/ESX-Org/esx_license [esx]/esx_license
```

### 手动
- 下载 https://github.com/ESX-Org/esx_license/archive/master.zip
- 解压至 `[esx]` 目录

## 安装
- 将 `esx_license.sql` 导入至你的数据库
- 添加下面这段设置至 `server.cfg`:

```
start esx_license
```

### Available triggers
- `'esx_license:addLicense', function(target, type, cb)`
- `'esx_license:removeLicense', function(target, type, cb)`
- `'esx_license:getLicense', function(source, cb, type)` (callback)
- `'esx_license:getLicenses', function(source, cb, target)` (callback)
- `'esx_license:checkLicense', function(source, cb, target, type)` (callback)
- `'esx_license:getLicensesList', function(source, cb)` (callback)
