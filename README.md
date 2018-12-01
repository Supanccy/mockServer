# mockServer使用注意事项

### 第一：mockServer运行说明
1. 命令行进入到moco-runner-0.11.1-standalone.jar所在的文件夹
2. 执行命令E:\WS_myself\mockServer>java -jar moco-runner-0.11.1-standalone.jar http -p 12306 -c foo.json
3. 用浏览器打开访问http://10.10.36.167:12306/hello即可

### 第二：json文件示例

```
[{
		"request": {
		    "method":"get",
			"uri": "/hello"
		},
		"response": {
			"text": "Hello World"
		}
	},
	{
		"request": {
		    "method":"get",
			"uri": "/go"
		},
		"response": {
			"text": "go away !!!"
		}
	}
]
```

### 第三：使用注意事项
1. json文件是要经过java解析的，所以json必须，必须，必须是标准的json格式。
2. json文件中不能有任何注释。
3. request里面的methos指定的什么方法，前台必须是什么请求。





