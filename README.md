# use guide
1、在maven的setting.xml中,<mirrorOf>标签中是*号的，要排除本仓库，如：
<mirror>
        <id>aliyun</id>
        <name>aliyun Maven</name>
        <mirrorOf>*,!gan-maven-repo</mirrorOf>
        <url>http://maven.aliyun.com/nexus/content/groups/public/</url>
</mirror>

2、在pom.xml中引入本仓库
'''
<repositories>
        <repository>
            <id>gan-maven-repo</id>
            <url>https://raw.githubusercontent.com/nicygan/maven-repository/master/repository</url>
        </repository>
</repositories>
'''
