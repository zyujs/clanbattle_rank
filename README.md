# clanbattle_rank

本项目为查询工会战排名信息的HoshinoBot插件,使用 [wiki.biligame.com](https://wiki.biligame.com/pcr/%E5%9B%A2%E9%98%9F%E6%88%98%E5%88%86%E6%95%B0%E6%9F%A5%E8%AF%A2%E5%B7%A5%E5%85%B7) API获取数据.

本项目地址 https://github.com/zyujs/clanbattle_rank

本项目适用于HoshinoBot v2

## 安装方法:

1. 在HoshinoBot的插件目录modules下clone本项目 `git clone https://github.com/zyujs/clanbattle_rank.git`
1. 在 `config/__bot__.py`的模块列表里加入 `clanbattle_rank`
1. 重启HoshinoBot

## 模块说明 :

本插件含有两个模块: 
- `clanbattle_rank` : 插件的基础功能
- `clanbattle_rank_push` : 每日工会战排名信息推送

其中推送功能仅在工会战期间推送信息, 分别为前6天的5:30和第7天的0:30, 如果不需要推送, 请自行关闭 `clanbattle_rank_push` 模块.

## 指令列表 :

- `查询排名 工会名 [工会id]` : 查询指定工会排名
- `查询分段` : 查询分段信息
- `查询关注` : 查询关注的工会信息
- `添加关注 工会名 [工会id]` : (需要管理员权限)将指定工会加入关注列表,如有重名需要附加工会id
- `清空关注` : (需要管理员权限)清空关注列表

例: 
```
查询排名 K.A.
查询排名 K.A. 44762
添加关注 K.A. 44762
查询关注
```

## 开源

本插件以GPL-v3协议开源
