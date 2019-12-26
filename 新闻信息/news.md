# industrynav-api
> 产业导航API

	全局api格式：http://xxx:xxx/xxx

**状态码：**
> 1. 418:账号未登录
> 2. 404:404错误

- 描述：全局大搜索框接口
- 地址：/base/getBaseByKeyword
- 类型：POST
- 数据类型：application/json
- 请求头：xxx

- 请求体：
```javascript
{
    "keyword":"农业"
}
	
```
- 响应

```javascript
{
    "msg":"成功",
    "code":1,
    "data":[
        {
            "materialStatus":-1,
            "sourceId":"5c4e9be742c1471b9dc38b4c",
            "classify":"A01XX000A",
            "website":"中华人民共和国国家邮政局",
            "keywords":[
                "GWYY-观点"
            ],
            "articleTime":1552917908784,
            "articleId":"5c8af47942c147038e0c9628",
            "title":"2019政府工作报告-国威永耀关注重点之四：【乡村振兴】",
            "userId":"5bf4402142c147574d2f945a",
            "content":"3月5日李克强总理在政府工作报告中提到，坚持农业农村优先发展，扎实推进乡村建设。科学编制建设规划，大力改善生产生活条件。加快实施农村饮水安全巩固提升工程，今明两年要解决好饮水困难人口的饮水安全问题，……。因地制宜开展农村人居环境整治，推进“厕所革命”、垃圾污水治理，建设美丽乡村。
            "recordTime":1552917908784,
            "surverdataId":"",
            "id":"5c8fa59442c147038e0d1221",
            "region":"NoData"
        },
        {
            "materialStatus":0,
            "sourceId":"",
            "classify":"A01XX000A",
            "website":"国威永耀观点",
            "keywords":[
                "GWYY-观点"
            ],
            "articleTime":1552838400000,
            "articleId":"",
            "link":"www.gwxll.com",
            "title":"2019政府工作报告-国威永耀关注重点：乡村振兴",
            "userId":"5bf4402142c147574d2f945a",
            "content":"3月5日李克强总理在政府工作报告中提到，坚持农业农村优先发展，扎实推进乡村建设。科学编制建设规划，大力改善生产生活条件。加快实施农村饮水安全巩固提升工程，今明两年要解决好饮水困难人口的饮水安全问题，……。因地制宜开展农村人居环境整治，推进“厕所革命”、垃圾污水治理，建设美丽乡村。
            "recordTime":1552919174983,
            "surverdataId":"",
            "id":"5c8faa8642c147038e0d12d1",
            "region":"NoData"
        }
    ]
}
```



- 描述：局部页面详细搜索   根据条件搜索 若无条件  则显示全部  参数可以按照需求传入
- 地址：/base/getBaseByCondition
- 类型：POST
- 数据类型：application/json
- 请求头：xxx

- 请求体：
```javascript
{
    "classify":"A01XX000A,1155545",   // 五级标签ids
    "region":"",            // 区域
    "startTime":"", // 开始时间  Long类型 时间戳 
    "endTime":""  // 结束时间  Long类型  时间戳
   
}
	
```
- 响应

```javascript
{
    "msg":"成功",
    "code":1,
    "data":[
        {
            "materialStatus":-1,
            "sourceId":"5c4e9be742c1471b9dc38b4c",
            "classify":"A01XX000A",
            "website":"中华人民共和国国家邮政局",
            "keywords":[
                "GWYY-观点"
            ],
            "articleTime":1552917908784,
            "articleId":"5c8af47942c147038e0c9628",
            "title":"2019政府工作报告-国威永耀关注重点之四：【乡村振兴】",
            "userId":"5bf4402142c147574d2f945a",
            "content":"3月5日李克强总理在政府工作报告中提到，坚持农业农村优先发展，扎实推进乡村建设。科学编制建设规划，大力改善生产生活条件。加快实施农村饮水安全巩固提升工程，今明两年要解决好饮水困难人口的饮水安全问题，……。因地制宜开展农村人居环境整治，推进“厕所革命”、垃圾污水治理，建设美丽乡村。
            "recordTime":1552917908784,
            "surverdataId":"",
            "id":"5c8fa59442c147038e0d1221",
            "region":"NoData"
        },
        {
            "materialStatus":0,
            "sourceId":"",
            "classify":"A01XX000A",
            "website":"国威永耀观点",
            "keywords":[
                "GWYY-观点"
            ],
            "articleTime":1552838400000,
            "articleId":"",
            "link":"www.gwxll.com",
            "title":"2019政府工作报告-国威永耀关注重点：乡村振兴",
            "userId":"5bf4402142c147574d2f945a",
            "content":"3月5日李克强总理在政府工作报告中提到，坚持农业农村优先发展，扎实推进乡村建设。科学编制建设规划，大力改善生产生活条件。加快实施农村饮水安全巩固提升工程，今明两年要解决好饮水困难人口的饮水安全问题，……。因地制宜开展农村人居环境整治，推进“厕所革命”、垃圾污水治理，建设美丽乡村。
            "recordTime":1552919174983,
            "surverdataId":"",
            "id":"5c8faa8642c147038e0d12d1",
            "region":"NoData"
        }
    ]
}
```


- 描述：通过新闻id获取到新闻详细信息
- 地址：/base/getById
- 类型：POST
- 数据类型：application/json
- 请求头：xxx

- 请求体：
```javascript
{
    "id":"5c87484342c1470b07191c28"
}
	
```
- 响应

```javascript
{
    "msg":"成功",
    "code":1,
    "data":{
        "materialStatus":0,
        "sourceId":"5c8622e942c1470b071902d4",  // 资源id
        "classify":"C3233006A",
        "website":"中央宣传部",
        "keywords":[      // 关键词   显示
            "城市更新"
        ],
        "articleTime":1552369731942,      // 日期  显示
        "articleId":"5c87057e42c1470b07191745",
        "title":"严要求实作风，再创时代伟业——写在“三严三实”提出五周年之际---中国文明网",   // 标题   显示
        "userId":"5bf43780d4187d2a7eb620de",
        "content":"新华社北京3月8日电（新华社记者王敏　张紫赟　胡浩　黄小希）5年前，习近平总书记在参加十二届全国人大二次会议安徽代表团审议时提出“三严三实”要求，强调各级领导干部都要树立和发扬好的作风，既严以修身、严以用权、严以律己，又谋事要实、创业要实、做人要实。",
        "recordTime":1552369731942,
        "surverdataId":"",
        "id":"5c87484342c1470b07191c28",
        "region":"120117"
    }
}
```