# maven-repo

```
mvn install:install-file -Dfile=${path}/${artifactId}.jar -DgroupId=com.github.7kgame -DartifactId=testlib -Dversion=1.0.0 -Dpackaging=jar

git add -f com/github/7kgame/${artifactId}

```
```
allprojects {
    repositories {
        jcenter()
            maven{
                url 'https://raw.githubusercontent.com/7kgame/maven-repo/master'
            }
    }
}

compile 'com.github.7kgame:testlib:1.0.0'
```

