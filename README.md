# spring-cloud-config-server-repo

1. `@EnableConfigServer`
```java

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.config.server.EnableConfigServer;

@SpringBootApplication
@EnableConfigServer //激活应用配置服务器
public class SpringCloudLesson3ConfigServerApplication {

	public static void main(String[] args) {
		SpringApplication.run(SpringCloudLesson3ConfigServerApplication.class, args);
	}
}
```
2. application.properties
```shell
# org.springframework.cloud.config.server.environment.MultipleJGitEnvironmentRepository
## 配置服务器远程 Git 仓库（GitHub）
spring.cloud.config.server.git.uri = https://github.com/liqxhx/spring-cloud-config-server-repo
## 强制拉去 Git 内容
spring.cloud.config.server.git.force-pull = true
```
