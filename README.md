# CacheToFile
CacheToFile is a java library to cache your data.
This library store your java object in to file system.so no worry about loss your data when server is restarted.  
# How to use
Create object :

    private CacheToFile cacheToFile = new CacheToFile("/Users/administrator/Downloads");
    
    if (cacheToFile.has("you key")) {
      out.println(cacheToFile.get("your key"));
      out.println("From cache");
    } else {
     //Some long operation 
     boolean cached = cacheToFile.put("your key", <your object>, <Cache unit>, <Unit value>);
    }
     
    out.println(cacheToFile.get("your key"));
    out.println("From not cache");
    }
# Cache unit
 1. CacheToFile.unit.DAY
 2. CacheToFile.unit.HOUR
 3. CacheToFile.unit.MINUTE
 
 # Unit value
 Provide valid Integer value

# Maven dependency
<repository>
    <id>com.cache</id>
    <url>https://github.com/mukeshdabhi/CacheToFile/blob/master/CacheToFile.jar</url>
</repository>
<dependency>
    <groupId>com.cache</groupId>
    <artifactId>Cache To File</artifactId>
    <version>1.0</version>
</dependency>
