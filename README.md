# maven-repo
My personal maven repository.

## Usage
pom.xml:
```xml
    <repositories>
        <repository>
            <id>maven</id>
            <url>https://raw.github.com/distantguang/maven/artifact/mvnrep</url>
        </repository>
    </repositories>
```

## publish
发布项目pom.xml配置：
```xml
  <distributionManagement>
    <repository>
      <id>maven</id>
      <url>file:///${maven项目的本地git库路径}/mvnrep</url>
    </repository>
  </distributionManagement>
```
执行idea工具的deploy命令,将mvnrep目录下的文件提交到git远程库中。
