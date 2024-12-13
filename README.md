- web.xml: cấu hình ứng dụng web của java
- <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>: chỉ ra file cấu hình Spring MVC là dispatcher-servlet.xml
- <url-pattern> nhận request trang nao gọi servlet đó
- dispatcher-servlet.xml: 
- cấu hình dành riêng cho ứng dụng Spring MVC.
- <context:component-scan base-package="com.example.springgreeting"/>: trỏ sang Controller
- <bean class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <property name="prefix" value="/WEB-INF/views/"/>
        <property name="suffix" value=".jsp"/>
    </bean>: trỏ sang view
- applicationContext.xml: 
- định nghĩa các bean được chia sẻ giữa các servlet.
- xsi:schemaLocation như kiểu import các package
- Nhìn vào controller: 
