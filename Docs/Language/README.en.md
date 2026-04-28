# Bedrock-Command-Collection

## Copyright&Disclaimer / 版权与免责声明
> [🇺🇸 English](Copyright-Disclaimer/README.en.md)｜[🇨🇳 简体中文](Copyright-Disclaimer/README.zh-cn.md)

## Language / 语言
> [🇺🇸 English](README.en.md)｜[🇨🇳 简体中文](https://github.com/inltree/Bedrock-Collection)

> [🔙 Back to Repository](https://github.com/inltree/Bedrock-Collection)

## Command Block Property Comparison Table
| Category | Option | Emoji |
| :--- | :--- | :--- |
| Block Type | Impulse | `🟠` |
| Block Type | Chain | `🟢` |
| Block Type | Repeat | `🟣` |
| Condition Type | Unconditional | `☑️` |
| Condition Type | Conditional | `✅` |
| Activation Mode | Redstone Controlled | `⭕` |
| Activation Mode | Always Active | `🔴` |
| Delay | Tick Delay | `⏳` |

## Format Template

- Emoji Template：
【<🟠/🟢/🟣>｜<☑️/✅>｜<⭕/🔴>｜⏳ <Value>】

- Text Template：
【<Impulse/Chain/Repeat>｜<Unconditional/Conditional>｜<Redstone Controlled/Always Active>｜Delay <Value>】

### Example Template

#### Exchange System
- Function：Consume items to exchange for other items!
- Last Modified：2026-04-28 22:32:15
    - [x] Original Author：[@inltree]()
    - [x] Source Link：[bilibili](#)
    - [x] Original Work
    - [x] Authorized
    - [x] Reference：[Minecraft Wiki](#) / [Bilibili](#)

- 1. 【🟠｜☑️｜⭕｜⏳ 0】
```command
execute as @p run titleraw @s title {"rawtext":[{"translate":"%%2","with":{"rawtext":[{"selector":"@s[hasitem={item=emerald,quantity=64..}]"},{"text":"§aExchange successful\n\n"},{"text":"§cExchange failed\n\n"}]}}]}
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
```commabd
give @p apple 64 0
```

### Format Combination Table

|No.|Emoji Format|Text Format|
|---|---|---|
|1|【🟠｜☑️｜⭕｜⏳ 0】|【Impulse｜Unconditional｜Redstone Controlled｜Delay 0】|
|2|【🟠｜☑️｜🔴｜⏳ 0】|【Impulse｜Unconditional｜Always Active｜Delay 0】|
|3|【🟠｜✅｜⭕｜⏳ 0】|【Impulse｜Conditional｜Redstone Controlled｜Delay 0】|
|4|【🟠｜✅｜🔴｜⏳ 0】|【Impulse｜Conditional｜Always Active｜Delay 0】|
|5|【🟢｜☑️｜⭕｜⏳ 0】|【Chain｜Unconditional｜Redstone Controlled｜Delay 0】|
|6|【🟢｜☑️｜🔴｜⏳ 0】|【Chain｜Unconditional｜Always Active｜Delay 0】|
|7|【🟢｜✅｜⭕｜⏳ 0】|【Chain｜Conditional｜Redstone Controlled｜Delay 0】|
|8|【🟢｜✅｜🔴｜⏳ 0】|【Chain｜Conditional｜Always Active｜Delay 0】|
|9|【🟣｜☑️｜⭕｜⏳ 0】|【Repeat｜Unconditional｜Redstone Controlled｜Delay 0】|
|10|【🟣｜☑️｜🔴｜⏳ 0】|【Repeat｜Unconditional｜Always Active｜Delay 0】|
|11|【🟣｜✅｜⭕｜⏳ 0】|【Repeat｜Conditional｜Redstone Controlled｜Delay 0】|
|12|【🟣｜✅｜🔴｜⏳ 0】|【Repeat｜Conditional｜Always Active｜Delay 0】|