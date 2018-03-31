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
&lt;repository&gt; <br/>
    &lt;id&gt;com.cache&lt;/id&gt;<br/>
    &lt;url&gt;https://github.com/mukeshdabhi/CacheToFile/blob/master/CacheToFile.jar &lt;/url&gt;<br/>
&lt;/repository&gt;<br/>
<br/>
&lt;dependency&gt;<br/>
    &lt;groupId&gt;com.cache&lt;/groupId&gt;<br/>
    &lt;artifactId&gt;Cache-To-File&lt;/artifactId&gt;<br/>
    &lt;version&gt;1.0&lt;/version&gt;<br/>
&lt;/dependency&gt;
