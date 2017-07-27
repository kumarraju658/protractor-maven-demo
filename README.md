# protractor-maven-demo

## Steps: 
- Create maven project
- Create specs and config folder under src->test
- Add build file under POM:
```<build>
		<plugins>
			<plugin>
				<groupId>com.github.greengerong</groupId>
				<artifactId>maven-ng-protractor</artifactId>
				<version>0.0.2</version>
				<configuration>
					<protractor>protractor</protractor>
					<configFile>src/test/js/config/config.js</configFile>
				</configuration>
				<executions>
					<execution>
						<id>ng-protractor</id>
						<phase>integration-test</phase>
						<goals>
							<goal>run</goal>
						</goals>
					</execution>
				</executions>
			</plugin>
		</plugins>
	</build>
```