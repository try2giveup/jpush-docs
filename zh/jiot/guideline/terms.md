# 名词释义

## 名词释义
###产品
一类具备相同属性设备的抽象定义。用于集中管理组织管理设备的集合。（逻辑地位可以类比为极光的开发者服务的 app）。产品通过开发者账号在产品管理页面创建生成，其核心信息是 Product key 

### 设备
属于产品的某个具体物联网设备。设备通过在产品的设备管理功能创建得到，不同的设备在创建的时候会分配对应的 deviceSecret 用于区分鉴权。

### 属性：
通过产品的属性定义页面添加设置，是物联网设备的通用的性质的抽象定义。如灯光的颜色，开关状态等。

### 事件
通过产品的属性定义页面添加设置，用于设备上报的运营中产生的各种事件。包括“信息”，“告警”，“故障”三种类型。事件允许用户传递自定义参数。

### topic 列表
一个设备下订阅和发布的全部 topic 的列表

### 设备影子
每个设备都会在云端有设备影子与其一一对应，用于同步存储设备属性和状态。客户端和服务端可以通过对应的接口查看和修改设备的属性。


##关系
一个账户下允许创建多个产品
一个产品下添加多个设备
一个设备对应一个设备影子
topic 类和属性事件定义都属于产品，设备级别不能调整。