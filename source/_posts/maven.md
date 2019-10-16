---
title: maven
date: 2019-09-29 20:07:44
tags: 
    - maven
comments: true
cover: http://pyjw54h3s.bkt.clouddn.com/193744-1557056264d7ed.jpg
description: some maven commands
---

### maven相关命令

#### maven项目版本设置
```bash
mvn versions:set -DnewVersion=xxx

mvn versions:commit
```

#### maven提交源码
添加plugin插件
```xml
<build>
		<plugins>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-source-plugin</artifactId>
				<version>${version}</version>
				<configuration>
					<attach>true</attach>
				</configuration>
				<executions>
					<execution>
						<phase>compile</phase>
						<goals>
							<goal>jar</goal>
						</goals>
					</execution>
				</executions>
			</plugin>
		</plugins>
	</build>
```