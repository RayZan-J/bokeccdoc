# Spark API 开发指南

## 创盛视联数码科技（北京）有限公司

### 目 录

#### 1. 概述 3

1. 通信约定 3

2.1 HTTP方法 3

2.2 返回格式 3

2.3 编码格式 3

2.4 加密 3

2.5 接口访问次数限制 4

1. HTTP接口 4

3.1 获取用户信息 4

```
<?xml version="1.0" encoding="UTF-8"?>
<error>ERROR_CODE</error>
```

| A | B | C |
| --- | --- | --- |
| 1 | 2 | 3 |

```
<script src="//view.csslcloud.net/js/jquery-1.9.0.min.js" type="text/javascript"></script>
```

```
<script type="text/javascript">
    DWLive.init({
        userid: 'userid',
        roomid: 'roomid',
        viewername: 'name',
        viewertoken: 'password',
        viewercustomua: 'android',
        language: 'en',
        viewercustominfo: '{"exportInfos": [ {"key": "城市", "value": "北京"}, {"key": "姓名", "value": "哈哈"}]}',
        fastMode:true
    });
</script>
```

```
onPublicChatMessage:
{
    "userid":"4ccd73b2fb1a4b63be1043b6c4c225dc", // 发送者id
    "username":"name",   // 发送者名字
    "userrole":"student",   // 发送者身份
    "useravatar":"img",   // 发送者头像
    "msg":"rrr",   // 消息内容
    "time":"16:45:08",   // 发送时间
    "usercustommark": ""  // 聊天自定义参数
}

onPrivateChatMessage:
{
    "fromuserid":"7a4715874d504b8db78cb5b77d66b8c8",  // 发送者id
    "fromusername":"name",   // 发送者名字
    "touserid":"33ed40d2d7b746919219789733b5bdd4",  // 接收者id
    "tousername":"第三方士大夫",   // 接收者名字
    "msg":"发反反复复",   // 消息内容
    "time":"17:22:15"   // 发送时间
}

onPrivateAnswer:
{
    "fromuserid":"33ed40d2d7b746919219789733b5bdd4",  // 发送者id
    "fromusername":"第三方士夫",  // 发送者名字
    "fromuserrole":"student",   // 发送者身份
    "touserid":"7a4715874d504b8db78cb5b77d66b8c8",  // 接收者id
    "tousername":"name",   // 接收者名字
    "msg":"阿斯蒂芬",   // 消息内容
    "time":"17:26:24"  // 发送时间
}

onQuestion:
{
    "action":"question",  // 提问
    "time":-1,
    "value":
    {
        "userId":"C783F0F7CB77E1F3",  // 提问者id
        "userName":"name",   // 提问者名字
        "content":"123145",  // 提问内容
        "userAvatar":"img",     // 提问者头像
        "id":"1B5BBA4826FFE337"   // 问题id
    }
}

onAnswer:
{
    "action":"answer",   // 回答
    "time":-1,
    "value":
    {
        "content":"ghghjgug",   // 回答内容
        "isPrivate":0,    // 是否仅提问者可见
        "questionId":"1B5BBA4826FFE337",   // 问题id
        "questionUserId":"C783F0F7CB77E1F3",   // 提问者id
        "userId":"ebadb3d414c3471786d095c93bab8cb5",  // 回答者id
        "userName":"www",   // 回答者名字
        "userAvatar":"img",    // 回答者头像
        "userRole":"publisher"   // 回答者身份
    }
}

onPageChange:
{
    "docId": "xxxx",//当前页id
    "docName": "Java.pdf",//当前页name
    "docTotalPage": 105,//总页数
    "pageNum": 0    //当前页索引值
}

onBroadcastMsg:
{
    content: "大家好",//广播内容
    time: 205 //广播时间
}

userRole和fromuserrole对应关系表示如下:
    unknow: 未知角色;
    publisher: 主讲;
    teacher: 助教;
    host: 主持人;
    student: 学员（观众1）;   
```



