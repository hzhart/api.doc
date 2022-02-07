# 雪花ID服务

## 生成雪花ID(Snowflake)

```
GET /genid/v1
```

> 请求参数:

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>size</td>
        <td>-</td>
        <td>数量, 默认: 1</td>
    </tr>
    <tr>
        <td>format</td>
        <td>-</td>
        <td>模式: dec: 十六进制 num:数字, 默认: num</td>
    </tr>
</table>
