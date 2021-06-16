# 常用环境变量备份表


## 个人隐私类变量

```
## 1、运行脚本时，是否显示log,默认显示，但会输出个人信息。
## 默认值为true，引号中填写false则不显示，注重隐私的人可以自行设置为false
export JD_DEBUG=""
```


## 通知类环境变量

```
## 1. ServerChan
export PUSH_KEY=""
```

```
## 2. BARK
export BARK_PUSH=""
export BARK_SOUND=""
```

```
## 3. Telegram
export TG_BOT_TOKEN=""
export TG_USER_ID=""
```

```
## 4. 钉钉
export DD_BOT_TOKEN=""
export DD_BOT_SECRET=""
```

```
## 5. iGot聚合推送。
export IGOT_PUSH_KEY=""
```

```
## 6. Push Plus
export PUSH_PLUS_TOKEN=""
export PUSH_PLUS_USER=""
```

```
## 7. 企业微信机器人消息推送 webhook 后面的 key
export QYWX_KEY=""
```

```
## 8. 企业微信应用消息推送的值
export QYWX_AM=""
```

```
## 9. go-cqhttp
## gobot_url 推送到个人QQ: http://127.0.0.1/send_private_msg  群：http://127.0.0.1/send_group_msg
## gobot_token 填写在go-cqhttp文件设置的访问密钥
## gobot_qq 如果GOBOT_URL设置 /send_private_msg 则需要填入 user_id=个人QQ 相反如果是 /send_group_msg 则需要填入 group_id=QQ群 
## go-cqhttp相关API https://docs.go-cqhttp.org/api
export GOBOT_URL=""
export GOBOT_TOKEN=""
export GOBOT_QQ=""
```


## 定义每日签到的通知形式

```
## js脚本每日签到提供3种通知方式，分别为：
## 关闭通知，那么请在下方填入0
## 简洁通知，那么请在下方填入1，其效果见：https://github.com/LXK9301/jd_scripts/blob/master/icon/bean_sign_simple.jpg
## 原始通知，那么请在下方填入2，如果不填也默认为2，内容比较长，这也是默认通知方式
NotifyBeanSign=""
```

## 定义每日签到每个接口间的延迟时间

```
## 默认每个签到接口并发无延迟，如需要依次进行每个接口，请自定义延迟时间，单位为毫秒，延迟作用于每个签到接口, 如填入延迟则切换顺序签到(耗时较长)
export JD_BEAN_STOP=""
```


## 脚本推送控制类环境变量

```
## 1、京东多合一签到脚本关闭运行结果推送，默认推送，填true表示不推送
export JD_BEAN_SIGN_STOP_NOTIFY=""
```

```
## 2、京东多合一签到脚本推送简单结果，默认推送完整版结果，填true表示启用简单推送
export JD_BEAN_SIGN_NOTIFY_SIMPLE=""
```

```
## 3、东东萌宠关闭推送。填写false为不关闭推送，true为关闭推送
export PET_NOTIFY_CONTROL=""
```

```
## 4、京东农场关闭推送。填写false为不关闭推送，true为关闭推送
export FRUIT_NOTIFY_CONTROL=""
```

```
## 5、京东领现金关闭推送。填写false为不关闭推送，true为关闭推送
export CASH_NOTIFY_CONTROL=""
```

```
## 6、京东摇钱树关闭推送。填写false为不关闭推送，true为关闭推送
export MONEYTREE_NOTIFY_CONTROL=""
```

```
## 7、京东点点券关闭推送。填写false为不关闭推送，true为关闭推送
export DDQ_NOTIFY_CONTROL=""
```

```
## 8、京东京东赚赚小程序关闭推送。填写false为不关闭推送，true为关闭推送
export JDZZ_NOTIFY_CONTROL=""
```

```
## 9、京东京东赚赚小程序关闭推送。填写false为不关闭推送，true为关闭推送
export JDZZ_NOTIFY_CONTROL=""
```

```
## 10、宠汪汪兑换京豆关闭推送。填写false为不关闭推送，true为关闭推送
export JDZZ_NOTIFY_CONTROL=""
```

```
## 11、宠汪汪赛跑获胜后是否推送通知。填false为不推送通知消息,true为推送通知消息
export JOY_RUN_NOTIFY=""
```

```
## 12、东东超市兑换奖品是否关闭推送通知。填false为不关闭推送,true为关闭推送
export JOY_RUN_NOTIFY=""
```

```
## 13、京喜财富岛控制是否运行脚本后通知。输入true为通知,不填则为不通知
export CFD_NOTIFY_CONTROL=""
```

```
## 14、京喜农场岛控制是否运行脚本后通知。0=只通知成熟;1=本次获得水滴>0;2=任务执行;3=任务执行+未种植种子
export JXNC_NOTIFY_LEVEL=""
```


## 功能配置类环境变量

```
## 1、京东领现金红包兑换京豆开关。false为不换,true为换(花费2元红包兑换200京豆，一周可换四次)，默认为false
export CASH_EXCHANGE=""
```

```
## 2、宠汪汪喂食数量。可以填的数字0,10,20,40,80,其他数字不可
export JOY_FEED_COUNT=""
```

```
## 3、宠汪汪帮好友喂食。false为不帮,true为帮
export JOY_HELP_FEED=""
```

```
## 4、宠汪汪是否赛跑(默认参加双人赛跑)。false为不跑,true为跑
export JOY_HELP_FEED=""
```

```
## 5、宠汪汪参加什么级别的赛跑。可选数字为2,10,50，
其中2代表参加双人PK赛，10代表参加10人突围赛，
50代表参加50人挑战赛(注：此项功能在JOY_RUN_FLAG为true的时候才生效)，
如若想设置不同账号参加不同类别的比赛则用&区分即可(如下三个账号：2&10&50)
export JOY_TEAM_LEVEL=""
```

```
## 6、宠汪汪赛跑自己账号内部互助。输入true为开启内部互助
export JOY_RUN_HELP_MYSELF=""
```

```
## 7、宠汪汪积分兑换多少京豆。目前可填值为20或者500,脚本默认0,0表示不兑换京豆
export JD_JOY_REWARD_NAME=""
```

```
## 8、东东超市兑换京豆数量。目前可输入值为20或者1000，或者其他商品的名称,例如碧浪洗衣凝珠
export MARKET_COIN_TO_BEANS=""
```

```
## 9、东东超市是否参加pk。true表示参加,false表示不参加
export JOIN_PK_TEAM=""
```

```
## 10、东东超市是否用金币抽奖。true表示抽奖,false表示不抽奖
export SUPERMARKET_LOTTERY=""
```

```
## 11、东东农场是否使用水滴换豆卡。true表示换,false表示不换
export FRUIT_BEAN_CARD=""
```

```
## 12、是否取关商品。环境变量内容的意思依次是是否取关全部商品(0表示一个都不),是否取关全部店铺数(0表示一个都不),遇到此商品不再进行取关,遇到此店铺不再进行取关
export UN_SUBSCRIBES=""
```

```
## 13、疯狂的JOY循环助力开关。true表示循环助力,false表示不循环助力，默认不开启循环助力
export JDJOY_HELPSELF=""
```

```
## 14、疯狂的JOY京豆兑换。0表示不换,其他按可兑换数填写。目前最小2000
export JDJOY_APPLYJDBEAN=""
```

```
## 15、疯狂的JOY购买joy等级。
export BUY_JOY_LEVEL=""
```

```
## 16、摇钱树是否卖出金果。true卖出，false不卖出，默认false
export MONEY_TREE_SELL_FRUIT=""
```

```
## 17、东东工厂心仪商品。
export FACTORAY_WANTPRODUCT_NAME=""
```

```
## 18、东东工厂控制哪个京东账号不运行此脚本。多个使用&连接
export JDFACTORY_FORBID_ACCOUNT=""
```

```
## 19、京喜工厂控制哪个京东账号不运行此脚本。多个使用&连接
export DREAMFACTORY_FORBID_ACCOUNT=""
```

```
## 20、0301脚本是否加购。如加设置true
export PURCHASE_SHOPS=""
```

```
## 21、京喜工厂拼团瓜分电力活动的activeId（当前需抓包替换或去群里求别人分享）
export TUAN_ACTIVEID=""
```


## 阿道夫部分环境变量

```
## 阿道夫脚本加购开关，填true加购
export ADOLF_ADDSKU=""
```

```
## 阿道夫脚本入会开关，填true入会
export ADOLF_MARTIN=""
```


## zoopanda部分环境变量

```
## zoopanda 与粽不同入会
export ZOO_OPENCAD="true"
```

```
## zoopanda 与粽不同加购
export ZOO_ADD2CART="true"
```


## 柠檬（胖虎部分环境变量）

```
## 是兄弟就来砍我脚本要参加砍价的商品ID
export actId="" 
```

```
## 是兄弟就来砍我脚本要要参加砍价的邀请码
export packetId="" 
```

```
## 省钱大赢家本期活动ID
export redEnvelopeId="" 
```

```
## 省钱大赢家邀请码
export inviter=""
```


## 青龙部分环境变量

```
## 1、在运行 ql repo 命令时，是否自动删除失效的脚本与定时任务
AutoDelCron="true"
```

```
## 2、由于github仓库拉取较慢，所以会默认添加代理前缀，如不需要请移除
GithubProxyUrl="https://ghproxy.com/"
```

```
## 3、设置定时任务执行的超时时间，默认1h，后缀"s"代表秒(默认值), "m"代表分, "h"代表小时, "d"代表天
CommandTimeoutTime="1h"
```

```
## 4、设置批量执行任务时的并发数，默认同时执行5个任务
MaxConcurrentNum="5"
```

```
## 5、在运行 task 命令时，随机延迟启动任务的最大延迟时间。
## 如果任务不是必须准点运行的任务，那么给它增加一个随机延迟，由你定义最大延迟时间，单位为秒，如 RandomDelay="300" ，表示任务将在 1-300 秒内随机延迟一个秒数，然后再运行
RandomDelay="300"
```

```
## 6、如果你自己会写shell脚本，并且希望在每次运行 ql update 命令时，额外运行你的 shell 脚本，请赋值为 "true"，默认为true
EnableExtraShell="true"
```

```
## 7、自动按顺序进行账号间互助（选填） 设置为 true 时，将直接导入code最新日志来进行互助
AutoHelpOther=""
```

```
## 8、定义 jcode 脚本导出的互助码模板样式（选填）
## 不填 使用“按编号顺序助力模板”，Cookie编号在前的优先助力
## 填 0 使用“全部一致助力模板”，所有账户要助力的码全部一致
## 填 1 使用“均等机会助力模板”，所有账户获得助力次数一致
## 填 2 使用“随机顺序助力模板”，本套脚本内账号间随机顺序助力，每次生成的顺序都不一致。
HelpType=""
```

```
## 9、是否自动启动bot，默认不启动，设置为true时自动启动，目前需要自行克隆bot仓库所需代码，存到ql/repo目录下，文件夹命名为dockerbot
AutoStartBot=""
```

```
## 10、安装bot依赖时指定pip源，默认使用清华源，如不需要源，设置此参数为空
PipMirror="https://pypi.tuna.tsinghua.edu.cn/simple"
```