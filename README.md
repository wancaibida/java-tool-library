# Java Tool Library

## tools.jar
### Platform: Linux
### Usage:
```
sudo java -classpath tools.jar sun.tools.jstack.JStack 25976
```

## ObjectSizeFetcherAgent.jar
Used for calculate java object size
### Usage:

Code:
```
long byteSize = ObjectSizeCalculator.getObjectSize([:])
println("Object size is ${byteSize / 1024 / 1024} mb")
```

Cli:

```
java -javaagent:ObjectSizeFetcherAgent.jar YOUR_CLASS_NAME
```