#
## Party类（玩家队伍管理器）

**处理玩家队伍**

| 内置变量  |说明 |
| :------------- | :----------: |
|`player`|玩家角色对象.|
|`members`|玩家队伍成员列表.|
|`version`|队伍版本(随着队伍成员的添加和移除发生变化).|


### 方法

| 方法  |说明 |
| :------------- | :----------: |
|[reset()](#reset)|重置队伍角色.|
|[createPlayer()](#createPlayer)|创建玩家角色.|
|[createMembers()](#createMembers)|创建玩家队伍成员.|
|[setPlayer()](#setPlayer)|设置玩家角色.|
|[addMember()](#addMember)|添加玩家队伍成员.|
|[removeMember()](#removeMember)|移除玩家队伍成员.|
|[shareInventory()](#shareInventory)|共享玩家角色包裹.|
|[saveData()](#saveData)|保存队伍角色数据.|
|[loadData()](#loadData)|加载队伍角色数据.|

### 方法详情

* <a name="reset">reset()</a>

说明：无参数，重置队伍角色

***

* <a name="createPlayer">createPlayer()</a>

说明：无参数，创建玩家角色

***

* <a name="createMembers">createMembers()</a>

说明：无参数，创建玩家队伍成员

***

* <a name="setPlayer">setPlayer(actor)</a>

| 参数  |类型|说明 |
| :------------- | :----------: | :----------: |
|actor|GlobalActor|玩家角色.|

说明：设置玩家角色

***

* <a name="addMember">addMember(actor)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|actor|GlobalActor|队伍成员.|

说明：添加玩家队伍成员

***

* <a name="removeMember">removeMember(actor)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|actor|GlobalActor|队伍成员.|

说明：移除玩家队伍成员

***

* <a name="shareInventory">shareInventory()</a>

说明：共享玩家角色包裹

***

* <a name="saveData">saveData()</a>

说明：保存队伍角色数据

***

* <a name="loadData">loadData(party)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|party|Object|party类型数据.|

说明：加载队伍角色数据

***



## Team类（势力队伍管理器）

**处理玩家队伍势力**

| 内置变量  |说明 |
| :------------- | :----------: |
|`key`|队伍的键(ID)列表.|
|`relationMaps`|队伍关系表(0:敌对, 1:友好).|
|`defaultId`|默认队伍键(ID).|


### 方法

| 方法  |说明 |
| :------------- | :----------: |
|[buildRelationMaps()](#buildRelationMaps)|构建角色队伍的关系映射表.|
|[isEnemy()](#isEnemy)|判断敌对关系.|
|[isFriendly()](#isFriendly)|判断友好关系.|
|[changeRelation()](#changeRelation)|改变角色队伍的关系.|
|[saveData()](#saveData)|保存队伍关系数据.|
|[loadData()](#loadData)|加载队伍关系数据.|

### 方法详情

* <a name="buildRelationMaps">buildRelationMaps(keys, code)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|key|string[]|队伍的ID列表.|
|code|string|队伍的关系代码.|

说明：构建角色队伍的关系映射表

***

* <a name="isEnemy">isEnemy()</a>

说明：判断敌对关系

***

* <a name="isFriendly">isFriendly()</a>

说明：判断友好关系

***

* <a name="changeRelation">changeRelation(teamId1, teamId2, relation)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|teamId1|string|队伍ID1.|
|teamId2|string|队伍ID2.|
|relation|number|队伍1和队伍2的关系(0:敌对, 1:友好).|

说明：改变角色队伍的关系

***

* <a name="saveData">saveData()</a>

说明：保存队伍关系数据

***

* <a name="loadData">loadData(team)</a>

| 参数  |类型|说明 |
| :------------- | :----------: |:----------: |
|team|object|team.|

说明：加载队伍关系数据

***









