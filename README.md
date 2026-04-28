# Bedrock-Command-Collection

## Copyright&Disclaimer / 版权与免责声明
> [🇺🇸 English](Docs/Copyright-Disclaimer/README.en.md)｜[🇨🇳 简体中文](Docs/Copyright-Disclaimer/README.zh-cn.md)

## Language / 语言
> [🇺🇸 English](Docs/Language/README.en.md)｜[🇨🇳 简体中文](README.md)

> [🔙 返回仓库](https://github.com/inltree/Bedrock-Command-Collection/)

### 命令方块属性对照表
| 类型 | 选项 | 表情 |
| :--- | :--- | :--- |
| 方块类型 | 脉冲 | `🟠` |
| 方块类型 | 连锁 | `🟢` |
| 方块类型 | 循环 | `🟣` |
| 条件类型 | 无条件 / 不受制约 | `☑️` |
| 条件类型 | 有条件 / 条件制约 | `✅` |
| 激活类型 | 红石控制 | `⭕` |
| 激活类型 | 保持开启 | `🔴` |
| 延迟 | 延迟数值 | `⏳` |

### 格式模板

- 表情模板：
【方块类型 <🟠/🟢/🟣>｜条件类型 <☑️/✅>｜激活类型 <⭕/🔴>｜⏳ <数值>】

- 文本模板：
【方块类型 <脉冲/连锁/循环>｜条件类型 <无条件/不受制约/有条件/条件制约>｜激活类型 <红石控制/保持开启>｜延迟 <数值>】

### 示例模板

#### 兑换系统
- 信息：使用物品进行兑换另一个物品！
- 修改时间：2026-04-28 22:32:15
    - [x] 原创作者：[@inltree]()
    - [x] 来源链接：[bilibili](#)
    - [x] 是否原创
    - [x] 是否授权
    - [x] 是否借鉴：[minecraft-wiki](#)/[bilibili](#)

- 1. 【🟠｜☑️｜⭕｜⏳ 0】
```command
execute as @p run titleraw @s title {"rawtext":[{"translate":"%%2","with":{"rawtext":[{"selector":"@s[hasitem={item=emerald,quantity=64..}]"},{"text":"§a兑换成功\n\n"},{"text":"§c兑换失败\n\n"}]}}]}
```
- 2. 【🟢｜☑️｜🔴｜⏳ 0】
```command
execute as @p run clear @s[hasitem={item=emerald,quantity=64..}] emerald 0 64
```
- 3. 【🟢｜✅｜🔴｜⏳ 0】
```command
playsound random.orb @p
```
- 4. 【🟢｜✅｜🔴｜⏳ 0】
```command
scoreboard players add @p "Coins" 0
```
- 5. 【🟢｜✅｜🔴｜⏳ 0】
```command
give @p apple 64 0
```

### 格式对照表

| 序号 | 表情格式 | 文本格式 |
| :---: | :--- | :--- |
| 1 | 【🟠｜☑️｜⭕｜⏳ 0】 | 【脉冲｜不受制约｜红石控制｜延迟 0】 |
| 2 | 【🟠｜☑️｜🔴｜⏳ 0】 | 【脉冲｜不受制约｜保持开启｜延迟 0】 |
| 3 | 【🟠｜✅｜⭕｜⏳ 0】 | 【脉冲｜条件制约｜红石控制｜延迟 0】 |
| 4 | 【🟠｜✅｜🔴｜⏳ 0】 | 【脉冲｜条件制约｜保持开启｜延迟 0】 |
| 5 | 【🟢｜☑️｜⭕｜⏳ 0】 | 【连锁｜不受制约｜红石控制｜延迟 0】 |
| 6 | 【🟢｜☑️｜🔴｜⏳ 0】 | 【连锁｜不受制约｜保持开启｜延迟 0】 |
| 7 | 【🟢｜✅｜⭕｜⏳ 0】 | 【连锁｜条件制约｜红石控制｜延迟 0】 |
| 8 | 【🟢｜✅｜🔴｜⏳ 0】 | 【连锁｜条件制约｜保持开启｜延迟 0】 |
| 9 | 【🟣｜☑️｜⭕｜⏳ 0】 | 【循环｜不受制约｜红石控制｜延迟 0】 |
| 10 | 【🟣｜☑️｜🔴｜⏳ 0】 | 【循环｜不受制约｜保持开启｜延迟 0】 |
| 11 | 【🟣｜✅｜⭕｜⏳ 0】 | 【循环｜条件制约｜红石控制｜延迟 0】 |
| 12 | 【🟣｜✅｜🔴｜⏳ 0】 | 【循环｜条件制约｜保持开启｜延迟 0】 |
