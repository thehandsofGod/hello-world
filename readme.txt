$.post("randomCode.s", function(data) 
#data �����������
#������������������.sΪ��׺�� ����

#����springmvc��mybatis�İ�
#SqlSessionFactory��MyBatis�Ĺؼ�����,���Ǹ��������ݿ�ӳ���ϵ�����������ڴ澵��
.SqlSessionFactory�����ʵ������ͨ��SqlSessionFactoryBuilder��������,
��SqlSessionFactoryBuilder����Դ�XML�����ļ���һ��Ԥ�ȶ��Ƶ�Configuration��ʵ��
������SqlSessionFactory��ʵ��.ÿһ��MyBatis��Ӧ�ó�����һ��SqlSessionFactory�����ʵ��
Ϊ����.ͬʱSqlSessionFactoryҲ���̰߳�ȫ��,SqlSessionFactoryһ��������,
Ӧ����Ӧ��ִ���ڼ䶼����.��Ӧ�������ڼ䲻Ҫ�ظ��������,����ʹ�õ���ģʽ.
SqlSessionFactory�Ǵ���SqlSession�Ĺ���.

<!-- ������ JDBC ֧���Զ��������������ɽ��Զ����ɵ��������ء� -->
<setting name="useGeneratedKeys" value="true"/>


#����������ʲô������������
ע�ⷽʽ����������ʲô������������������

#û��spring��mybatis���м��
#û�е���common-pool����dataSource�޷���ʵ��bean

Failed to introspect Class [org.springframework.web.multipart.commons.CommonsMultipartResolver] from ClassLoader [ParallelWebappClassLoader
#û�е���common-io.jar.ʵ���ļ��ϴ�������
#common-fileupdate.jar�Ǹ���

UsersDao����mybatis��Mapper����ӳ��ӿڣ�

Error creating bean with name 'usersController': Unsatisfied dependency expressed through field 'deptsService'; 
nested exception is org.springframework.beans.factory.NoSuchBeanDefinitionException:
No qualifying bean of type 'com.service.DeptsService' available: expected at least 1 bean which qualifies as autowire candidate. 
Dependency annotations: {@org.springframework.beans.factory.annotation.Autowired(required=true)}
	at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor$AutowiredFieldElement.inject(AutowiredAnnotationBeanPostProcessor.java:587)
#:�ǲ�֪��usersController�е�detsServiceû��ʵ�������ʸ�����Ϊû����DeptsService��ʵ�����м���ע��
#��Ȼ�������ļ��л�Ҫ�����Զ�ɨ��ע������ʣ�


//$.post()����ͨ�� HTTP POST ��ʽ��������������󲢻�ȡ���ص�����

#$.post({url:})�Դ��Ͷ���ķ�ʽ���̨�������ݣ����磬user����