# Websocket服务

## 登录服务器

```
wss://域名/ws
```

> 请求参数: 

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>id</td>
        <td>是</td>
        <td>用户id</td>
    </tr>
    <tr>
        <td>name</td>
        <td>是</td>
        <td>用户名</td>
    </tr>
    <tr>
        <td>domain</td>
        <td>是</td>
        <td>域</td>
    </tr>
    <tr>
        <td>resource</td>
        <td>是</td>
        <td>资源</td>
    </tr>
    <tr>
        <td>token</td>
        <td>是</td>
        <td>当前项目token</td>
    </tr>
</table>

## 发送消息

> 请求参数: 

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>toId</td>
        <td>是</td>
        <td>接收用户id</td>
    </tr>
    <tr>
        <td>type</td>
        <td>是</td>
        <td>消息类型, 10:文字消息 20:图片 30:语音 40:音视频 100:系统消息</td>
    </tr>
    <tr>
        <td>content</td>
        <td>是</td>
        <td>消息内容</td>
    </tr>
</table>

## 消息内容

<table>
    <tr>
        <th>参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>fromId</td>
        <td>是</td>
        <td>发送人id</td>
    </tr>
    <tr>
        <td>fromName</td>
        <td>是</td>
        <td>发送人姓名</td>
    </tr>
    <tr>
        <td>fromResource</td>
        <td>是</td>
        <td>发送人资源</td>
    </tr>
    <tr>
        <td>toId</td>
        <td>是</td>
        <td>接收用户id</td>
    </tr>
    <tr>
        <td>domain</td>
        <td>是</td>
        <td>域名</td>
    </tr>
    <tr>
        <td>type</td>
        <td>是</td>
        <td>消息类型, 10:文字消息 20:图片 30:语音 40:音视频 100:系统消息</td>
    </tr>
    <tr>
        <td>content</td>
        <td>是</td>
        <td>消息内容</td>
    </tr>
    <tr>
        <td>sendAt</td>
        <td>是</td>
        <td>原始发送时间</td>
    </tr>
    <tr>
        <td>offline</td>
        <td>是</td>
        <td>是否离线消息</td>
    </tr>
</table>

## 消息历史

```
GET /message-log
```

> 请求参数: 

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>domain</td>
        <td>是</td>
        <td>域</td>
    </tr>
    <tr>
        <td>toId</td>
        <td>是</td>
        <td>接收用户id</td>
    </tr>
    <tr>
        <td>fromId</td>
        <td>-</td>
        <td>发送人</td>
    </tr>
    <tr>
        <td>page</td>
        <td>-</td>
        <td>页码, 默认: 1</td>
    </tr>
    <tr>
        <td>size</td>
        <td>-</td>
        <td>每页大小, 默认: 10</td>
    </tr>
</table>

## 测试工具: https://websocketking.com/
