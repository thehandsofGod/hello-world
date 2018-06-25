$.post("randomCode.s", function(data) 
#data 是哪里的数据
#配置拦截器，拦截以.s为后缀的 请求

#导入springmvc和mybatis的包
#SqlSessionFactory是MyBatis的关键对象,它是个单个数据库映射关系经过编译后的内存镜像
.SqlSessionFactory对象的实例可以通过SqlSessionFactoryBuilder对象类获得,
而SqlSessionFactoryBuilder则可以从XML配置文件或一个预先定制的Configuration的实例
构建出SqlSessionFactory的实例.每一个MyBatis的应用程序都以一个SqlSessionFactory对象的实例
为核心.同时SqlSessionFactory也是线程安全的,SqlSessionFactory一旦被创建,
应该在应用执行期间都存在.在应用运行期间不要重复创建多次,建议使用单例模式.
SqlSessionFactory是创建SqlSession的工厂.

<!-- 则允许 JDBC 支持自动生成主键，并可将自动生成的主键返回。 -->
<setting name="useGeneratedKeys" value="true"/>


#事务配置是什么？？？？？？
注解方式配置事物是什么？？？？？？？？？

#没有spring和mybatis的中间包
#没有导入common-pool代理，dataSource无法是实现bean

Failed to introspect Class [org.springframework.web.multipart.commons.CommonsMultipartResolver] from ClassLoader [ParallelWebappClassLoader
#没有导入common-io.jar.实现文件上传输入流
#common-fileupdate.jar是更新

UsersDao就是mybatis的Mapper方法映射接口；

Error creating bean with name 'usersController': Unsatisfied dependency expressed through field 'deptsService'; 
nested exception is org.springframework.beans.factory.NoSuchBeanDefinitionException:
No qualifying bean of type 'com.service.DeptsService' available: expected at least 1 bean which qualifies as autowire candidate. 
Dependency annotations: {@org.springframework.beans.factory.annotation.Autowired(required=true)}
	at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor$AutowiredFieldElement.inject(AutowiredAnnotationBeanPostProcessor.java:587)
#:是不知道usersController中的detsService没有实例化的资格，是因为没有在DeptsService的实现类中加入注解
#当然在配置文件中还要加入自动扫面注解的性质；


//$.post()方法通过 HTTP POST 方式向服务器发送请求并获取返回的数据

#$.post({url:})以传送对象的方式向后台传送数据，比如，user，而