### nest使用MVC架构实现
#### Controller处理路由和解析请求参数
* 通过@Param取url中的请求参数，如user/111
* 通过@Query取url中的query请求参数，如user/xx?id=222
* 通过@Body取book/create中的请求体内容，通过dto(data transfer object)接收

#### service业务逻辑基本实现
* service实现了Ioc（Inverse of Control反转控制）
* 依赖注入的两种方式
  * 写在@Inject(JwtService)中的叫做属性注入
  * 写在构造器中的注入叫构造器注入

### nest cli命令
#### 全局安装nest cli命令
* `npm install -g @nestjs/cli`
* 需要及时更新`npm update -g @nestjs/cli`
#### nest命令自动生成模块
* 生成module`nest generate module aaa`
* 生成controller`nest generate controller aaa`
* 生成service`nest generate service aaa`
* 生成一个模块代码`nest generate resource xxx`
  * 选择生成REST风格API，选择CRUD

### 五种HTTP数据传输方式
* url param
* query
* form-urlencoded
* form-data
* json