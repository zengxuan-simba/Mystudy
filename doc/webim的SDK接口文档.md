<a name="module_RCSSdk"></a>

## RCSSdk
RCSSdk module


* [RCSSdk](#module_RCSSdk)
    * _static_
        * [.store](#module_RCSSdk.store)
        * [.rcsV6ListenerCallback](#module_RCSSdk.rcsV6ListenerCallback)
        * [.getSessionIdAsync()](#module_RCSSdk.getSessionIdAsync)
        * [.getLoginStatus(epid, sessionId)](#module_RCSSdk.getLoginStatus) ⇒
        * [._DoLogin()](#module_RCSSdk._DoLogin) ⇒ <code>object</code>
        * [._AuthAndLogin()](#module_RCSSdk._AuthAndLogin) ⇒ <code>object</code>
        * [._ReLogin()](#module_RCSSdk._ReLogin) ⇒ <code>object</code>
        * [._OneClickLogin(asToken)](#module_RCSSdk._OneClickLogin)
        * [._qrLogin(credentials)](#module_RCSSdk._qrLogin) ⇒ <code>object</code>
        * [._smsLogin(credentials)](#module_RCSSdk._smsLogin) ⇒ <code>object</code>
        * [.uploadMsg(msg, contentType, cb)](#module_RCSSdk.uploadMsg)
        * [.ready_recvmsg()](#module_RCSSdk.ready_recvmsg)
        * [.mqttReDial()](#module_RCSSdk.mqttReDial)
        * [.mqttQuit()](#module_RCSSdk.mqttQuit)
        * [.getSmsCode(tel)](#module_RCSSdk.getSmsCode)
        * [.smsProvisioning(epid, tel, searchVal, loginType)](#module_RCSSdk.smsProvisioning)
        * [.rcsDownloadPortrait(jsonParam, cb)](#module_RCSSdk.rcsDownloadPortrait) ⇒
        * [.getLastestContact(jsonParam, cb)](#module_RCSSdk.getLastestContact) ⇒
        * [.getContactList(jsonParam, cb)](#module_RCSSdk.getContactList)
        * [.getGroupList(jsonParam, cb)](#module_RCSSdk.getGroupList)
        * [.addressbook_List(jsonParam, cb)](#module_RCSSdk.addressbook_List) ⇒
        * [.getGroupMembers(jsonParam, cb)](#module_RCSSdk.getGroupMembers) ⇒
        * [.getAddressbookProfile(uriArrayList, cb)](#module_RCSSdk.getAddressbookProfile)
        * [.getContactInfo(jsonParam, cb)](#module_RCSSdk.getContactInfo) ⇒
        * [.exist()](#module_RCSSdk.exist)
        * [.destroyPicUploader()](#module_RCSSdk.destroyPicUploader)
        * [.initPicUploader()](#module_RCSSdk.initPicUploader)
        * [.unRegister()](#module_RCSSdk.unRegister)
    * _inner_
        * [~doLogin(jsonParam, cb)](#module_RCSSdk..doLogin)
        * [~getV6ConfigRelated(jsonParam, cb)](#module_RCSSdk..getV6ConfigRelated) ⇒ <code>Promise.&lt;any&gt;</code>
        * [~getUserInfo(cb)](#module_RCSSdk..getUserInfo)

<a name="module_RCSSdk.store"></a>

### RCSSdk.store
sdk内部store

**Kind**: static property of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.rcsV6ListenerCallback"></a>

### RCSSdk.rcsV6ListenerCallback
rcsV6ListenerCallback 初始化

**Kind**: static property of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.getSessionIdAsync"></a>

### RCSSdk.getSessionIdAsync()
获取SessionId

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.getLoginStatus"></a>

### RCSSdk.getLoginStatus(epid, sessionId) ⇒
**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 返回登录状态  

| Param |
| --- |
| epid | 
| sessionId | 

<a name="module_RCSSdk._DoLogin"></a>

### RCSSdk.\_DoLogin() ⇒ <code>object</code>
以默认方式登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: <code>object</code> - 以默认方式登录的结果  
<a name="module_RCSSdk._AuthAndLogin"></a>

### RCSSdk.\_AuthAndLogin() ⇒ <code>object</code>
手动开户成功后登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: <code>object</code> - 手动开户后登录的结果  
<a name="module_RCSSdk._ReLogin"></a>

### RCSSdk.\_ReLogin() ⇒ <code>object</code>
被踢下线后, 重新登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: <code>object</code> - 重新登录的结果  
<a name="module_RCSSdk._OneClickLogin"></a>

### RCSSdk.\_OneClickLogin(asToken)
单点登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| asToken | <code>object</code> | {astoken} return {object} 单点登录结果 |

<a name="module_RCSSdk._qrLogin"></a>

### RCSSdk.\_qrLogin(credentials) ⇒ <code>object</code>
二维码方式登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: <code>object</code> - 二维码登录的结果  

| Param | Type | Description |
| --- | --- | --- |
| credentials | <code>object</code> | {userId, mobileNo, credential} |

<a name="module_RCSSdk._smsLogin"></a>

### RCSSdk.\_smsLogin(credentials) ⇒ <code>object</code>
短验方式登录

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: <code>object</code> - 短验登录的结果  

| Param | Type |
| --- | --- |
| credentials | <code>object</code> | 

<a name="module_RCSSdk.uploadMsg"></a>

### RCSSdk.uploadMsg(msg, contentType, cb)
uploadMsg

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Description |
| --- | --- |
| msg | contentType callback() |
| contentType |  |
| cb | 回调函数 |

<a name="module_RCSSdk.ready_recvmsg"></a>

### RCSSdk.ready\_recvmsg()
消息订阅

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.mqttReDial"></a>

### RCSSdk.mqttReDial()
重连mqtt

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.mqttQuit"></a>

### RCSSdk.mqttQuit()
断开mqtt

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.getSmsCode"></a>

### RCSSdk.getSmsCode(tel)
获取短信验证码

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Description |
| --- | --- |
| tel | 手机号码格式:+8618610292748 |

<a name="module_RCSSdk.smsProvisioning"></a>

### RCSSdk.smsProvisioning(epid, tel, searchVal, loginType)
短信验证码登录--终端认证或开通请求 （已弃用）

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Description |
| --- | --- |
| epid |  |
| tel | 手机号码格式:+8618610292748 |
| searchVal | 短信验证码 |
| loginType | 登录类型 短信下行登录:3 |

<a name="module_RCSSdk.rcsDownloadPortrait"></a>

### RCSSdk.rcsDownloadPortrait(jsonParam, cb) ⇒
拉取头像

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 拉取头像结果  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | {mobile, size} |
| cb |  | 回调函数 |

<a name="module_RCSSdk.getLastestContact"></a>

### RCSSdk.getLastestContact(jsonParam, cb) ⇒
拉取最近联系人列表

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 最近联系人列表  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | {configversion: '0'} |
| cb |  | 回调函数 |

<a name="module_RCSSdk.getContactList"></a>

### RCSSdk.getContactList(jsonParam, cb)
获取联系人列表

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | { contactlistversion = 0 } |
| cb | <code>function</code> | 回调函数 |

<a name="module_RCSSdk.getGroupList"></a>

### RCSSdk.getGroupList(jsonParam, cb)
获取群列表

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | {configversion: '0'} |
| cb | <code>function</code> | 回调函数 |

<a name="module_RCSSdk.addressbook_List"></a>

### RCSSdk.addressbook\_List(jsonParam, cb) ⇒
获取通讯录列表

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 获取通讯录列表结果  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | {version: '0'} |
| cb |  | 回调函数 |

<a name="module_RCSSdk.getGroupMembers"></a>

### RCSSdk.getGroupMembers(jsonParam, cb) ⇒
获取群详情以及成员列表

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 获取群成员列表列表结果  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | { groupuri, groupinfoversion } |
| cb |  | 回调函数 |

<a name="module_RCSSdk.getAddressbookProfile"></a>

### RCSSdk.getAddressbookProfile(uriArrayList, cb)
获取通讯录资料

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| uriArrayList | <code>Array</code> |  |
| cb |  | 回调函数 |

<a name="module_RCSSdk.getContactInfo"></a>

### RCSSdk.getContactInfo(jsonParam, cb) ⇒
获取联系人详细资料

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
**Returns**: 获取联系人详细资料结果  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | { uri } |
| cb |  | 回调函数 |

<a name="module_RCSSdk.exist"></a>

### RCSSdk.exist()
检查待上传的图片是否已存在服务器上

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.destroyPicUploader"></a>

### RCSSdk.destroyPicUploader()
**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.initPicUploader"></a>

### RCSSdk.initPicUploader()
插件链接
https://github.com/flowjs/flow.js

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk.unRegister"></a>

### RCSSdk.unRegister()
注销登陆

**Kind**: static method of [<code>RCSSdk</code>](#module_RCSSdk)  
<a name="module_RCSSdk..doLogin"></a>

### RCSSdk~doLogin(jsonParam, cb)
登录

**Kind**: inner method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>Object</code> | 登录需要的参数对象 |
| cb | <code>function</code> | 回调函数 |

<a name="module_RCSSdk..getV6ConfigRelated"></a>

### RCSSdk~getV6ConfigRelated(jsonParam, cb) ⇒ <code>Promise.&lt;any&gt;</code>
获取手机免打扰设置详情

**Kind**: inner method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| jsonParam | <code>object</code> | { version } |
| cb |  | 回调函数 |

<a name="module_RCSSdk..getUserInfo"></a>

### RCSSdk~getUserInfo(cb)
获取我的个人信息

**Kind**: inner method of [<code>RCSSdk</code>](#module_RCSSdk)  

| Param | Type | Description |
| --- | --- | --- |
| cb | <code>function</code> | callback |

