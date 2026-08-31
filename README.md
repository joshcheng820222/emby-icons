# emby-icons

自用 Emby 服务器图标库，格式对齐 [xiyuliu509/Player-Icon](https://github.com/xiyuliu509/Player-Icon)。

## 播放器接入

在 SenPlayer / EPlayerX 的图标库设置里填：

```
https://raw.githubusercontent.com/joshcheng/emby-icons/refs/heads/master/invisible.json
```

## 结构

```
invisible.json          # 图标索引（播放器读取的入口）
icon/invisible/         # 图标文件，透明 PNG，512x512
```

## 加新图标

1. 透明 PNG 放进 `icon/invisible/`，文件名用小写英文/短横线
2. `invisible.json` 的 `icons` 里加一条 `{name, url}`，按名称 A-Z 排列
3. 提交后 `raw.githubusercontent.com` 地址即时生效（无缓存问题，客户端刷新即取）
