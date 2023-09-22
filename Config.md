# 配置

## 全局配置

1.推送样式

> 动态的推送样式 可配置选项：\[绘图]\[标题]\[链接]\[内容]\[图片]

```markup
bilipush_push_style="[绘图][标题][链接]"
```

2.刷新间隔：

> 每次刷新间隔多少分钟，默认为 12 分钟。

```markup
bilipush_waittime=12
```

3.发送间隔：

> 每次发送完成后等待的时间，单位秒，默认 10-30 秒。 时间为设置的时间再加上随机延迟 1-20 秒

```markup
bilipush_sleeptime=10
```

4.最大发送数量

> 限制单次发送数量，防止一次性发送太多图导致风控。 默认 5 条

```markup
bilipush_maximum_send=5

```

5.其他配置项

> 只响应一个 bot 一个群内有多个 bot，可以只让 1 个 bot 推送消息。 默认为关闭该功能，既所有 bot 都会响应 （正在考虑是否改为默认开启，如不需要请关闭该功能）

```markup
bilipush_botswift=False
```

> 是否使用花音的 api 来支持更丰富的内容
>
> 默认开启。如出现连接不上或其他故障，请尝试关闭。

```markup
bilipush_emojiapi=True
```

> 配置 api 地址，如未填写则使用默认地址。

```markup
bilipush_apiurl="http://cdn.kanon.ink"
```

## 群内配置项（beta）

（正在内测功能，并未正式上线

```markup
# 设置的群号
[g123456789]
# 配置项。如不存在则按照默认配置
group_admin=["123456", "111111", "222222"]
# 配置项。如不存在则按照默认配置
bilipush_push_style="[绘图][标题][链接]"
# at所有成员。默认关闭
at_all=False
```
