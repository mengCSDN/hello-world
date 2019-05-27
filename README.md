# 活动相关接口

### 索引
1. [新增活动](#新增活动)
2. [删除活动](#删除活动)
3. [修改活动](#修改活动)
4. [活动列表](#活动列表)
5. [活动详情](#活动详情)

### 新增活动
   
* 接口地址：/activity/add
* 接口说明：新增活动
* 请求类型：post
* 请求参数：
* 
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityName | String |否 |活动名称 |
| activityType | int |否 |活动类型:1拼团 2秒杀 3预售 4抽奖 |
| invitation   | int |否 |邀请人数 |
| lotteryCondition | int |否 |开奖条件(新人数) |
| winningNumber | int |否 |中奖数量（单次） |
| startAt | String |否 |开始时间 "yyyy-MM-dd HH:mm:ss"|
| endAt | String |否 |结束时间 "yyyy-MM-dd HH:mm:ss"|
| skuID | int |否 |商品ID |
| freight | String |否 |运费 |
| Status | int |否 |状态（-1:关闭 0:开启）|
*  
*  返回参数:无

### 删除活动
   
* 接口地址：/activity/delete
* 接口说明：删除活动
* 请求类型：post
* 请求参数：
* 
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityId | int |否 |活动Id |

*  返回参数:无

### 修改活动
   
* 接口地址：/activity/update
* 接口说明：修改活动
* 请求类型：post
* 请求参数：
* 
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityId | int |否 |活动Id |
| activityName | String |是 |活动名称 |
| activityType | int |是 |活动类型:1拼团 2秒杀 3预售 4抽奖 |
| invitation   | int |是 |邀请人数 |
| lotteryCondition | int |是 |开奖条件(新人数) |
| winningNumber | int |是 |中奖数量（单次） |
| startAt | String |是 |开始时间 "yyyy-MM-dd HH:mm:ss"|
| endAt | String |是 |结束时间 "yyyy-MM-dd HH:mm:ss"|
| skuID | int |是 |商品ID |
| freight | String |是 |运费 |
| Status | int |是 |状态（-1:关闭 0:开启）|
*  
*  返回参数:无

### 活动列表
   
* 接口地址：/activity/list
* 接口说明：活动列表
* 请求类型：post
* 请求参数：无
*  返回参数:
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityName | int |是 |活动名称 |
| activityType | int |是 |活动类型 |

*  返回参数:
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityId | int |否 |活动Id |
| activityName | String |否 |活动名称 |
| productUrl | String |否 |商品图片 |
| activityType | int |否 |活动类型:1拼团 2秒杀 3预售 4抽奖 |
| winningNumber | int |否 |中奖数量（单次） |
| startAt | String |否 |开始时间 "yyyy-MM-dd HH:mm:ss"|
| endAt | String |否 |结束时间 "yyyy-MM-dd HH:mm:ss"|
| skuID | int |否 |商品ID |
| quantity | int |否 |库存 |
| countMember | int |否 |累计新人 |
| newMemberCount | int |否 |本场新人数 |
| memberCount | int |否 |参与总人数 |
| creatAt | String |否 |发布时间 "yyyy-MM-dd HH:mm:ss" |
| status | int |否 |状态（-1:关闭 0:开启）|
* 

### 活动详情
   
* 接口地址：/activity/details
* 接口说明：活动详情
* 请求类型：post
* 请求参数：
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityId | int |否 |活动Id |
* 

*  返回参数:
| 参数 |类型 | 是否可空 | 参数说明 |
|-----|-----|---------|-----|
| activityId | int |否 |活动Id |
| activityName | String |是 |活动名称 |
| activityType | int |是 |活动类型:1拼团 2秒杀 3预售 4抽奖 |
| invitation   | int |是 |邀请人数 |
| lotteryCondition | int |是 |开奖条件(新人数) |
| winningNumber | int |是 |中奖数量（单次） |
| startAt | String |是 |开始时间 "yyyy-MM-dd HH:mm:ss"|
| endAt | String |是 |结束时间 "yyyy-MM-dd HH:mm:ss"|
| skuID | int |是 |商品ID |
| freight | String |是 |运费 |
| Status | int |是 |状态（-1:关闭 0:开启）|
* 