# drift-bottle

NodeJS漂流瓶应用，本项目基于 Express  Redis  MongoDB 

## 如何使用

`npm install && bower install`

### 如何运行

1、首先，需要运行 _Redis_ 服务：

	$ redis-server
	
2、然后，启动 _MongoDB_ 数据库：

  $ mongod --dbpath="D:\soft\mongodb-5.0.5\data"            // 本地
	
	$ ./mongod -f /usr/local/mongodb410/bin/mongodb.conf      // 远程
	
3、最后，运行 _Express_ 应用:

    ./bin/www

### 网页访问
1、访问地址（比较慢）：``` http://106.75.75.186:3000/ ```

### 接口测试
1、扔一个漂流瓶  
- 请求地址：`http://106.75.75.186:3000/throw.do`
- 请求参数：
  ```JSON
    {
      "time": 1640437976000,
      "owner": "cjk12",
      "type": "0",
      "content": "扔一个瓶子999"
    }
  ```
- 响应数据：
  ```JSON
    {
        "code": 1,
        "msg": "OK"
    }
  ```
2、捡一个漂流瓶  
- 请求地址：`http://106.75.75.186:3000/throw.do`
- 请求参数：
  ```JSON
    {
      "time": 1640437976000,
      "owner": "cjk12",
      "type": "0",
      "content": "扔一个瓶子999"
    }
  ```
- 响应数据：
  ```JSON
    {
        "code": 1,
        "msg": "OK"
    }
  ```

