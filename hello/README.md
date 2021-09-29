## Docker Command for Dockerfile

```
docker build -t yog3shwar/hello-api:dockerfile1 .
```

## Dockerfile-maven spotify plugin

This plugin will build a docker image whenever the `mvn package` command is ran

```
<plugin>
	<groupId>com.spotify</groupId>
	<artifactId>dockerfile-maven-plugin</artifactId>
	<version>1.4.10</version>
	<executions>
		<execution>
			<id>default</id>
			<goals>
				<goal>build</goal>
			</goals>
	    </execution>
	</executions>
	<configuration>
        <repository>yog3shwar/${project.name}</repository>
		<tag>${project.version}</tag>
		<skipDockerInfo>true</skipDockerInfo>
		</configuration>
</plugin>
```
