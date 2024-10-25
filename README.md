### nest使用MVC架构实现
#### Controller
* 通过@Param取url中的请求参数，如user/111
* 通过@Query取url中的query请求参数，如user/xx?id=222
* 通过@Body取book/create中的请求体内容，通过dto(data transfer object)接收