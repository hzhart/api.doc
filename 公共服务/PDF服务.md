# PDF服务

## PDF转图片

```
GET /pdf2img/v1/pdf2png
```

> 请求参数:

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>pdf</td>
        <td>是</td>
        <td>pdf网址</td>
    </tr>
</table>

## PDF生成服务

```
POST /genpdf/v1
```

> 请求参数:

<table>
    <tr>
        <th>请求参数</th>
        <th>必须</th>
        <th>说明</th>
    </tr>
    <tr>
        <td>url</td>
        <td>-</td>
        <td>要生成pdf的网页</td>
    </tr>
    <tr>
        <td>html</td>
        <td>-</td>
        <td>要生成pdf的html, url和html二选一/td>
    </tr>
    <tr>
        <td>pageSize</td>
        <td>-</td>
        <td>页面大小, 默认: A4/td>
    </tr>
    <tr>
        <td>orientation</td>
        <td>-</td>
        <td>页面方向, 默认: Portrait, 可选: Landscape</td>
    </tr>
    <tr>
        <td>dpi</td>
        <td>-</td>
        <td>DPI, 默认: 300</td>
    </tr>
</table>
