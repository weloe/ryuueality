SpringBoot

@Configuration

属性proxyBeanMethods默认true

是不是代理bean的方法 

true容器中保存的是这个类的代理对象，调用方法是代理的方法 调用方法会根据name检查返回的Bean在容器中有没有，如果有，获取容器Bean时会去容器中查找这个Bean并返回，保证单例，用于组件依赖

Full(``=true)

Lite(```=false)

只是注册组件，但组件之间没有依赖关系，用false，同时也少了检查步骤，速度更快





@SpringBootApplication

这个注解有@SpringBootConfiguration





@MatrixVariable

获取矩阵变量

springboot默认禁用获取矩阵变量的功能，要手动开启：

对于路径的处理，UrilPathHelper进行解析，

removeSemicolonContent(默认移除分号后面的内容)，改成false不移除，才能获取矩阵变量
