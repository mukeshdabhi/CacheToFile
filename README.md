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
      cacheToFile.put("your key", <your object>, CacheToFile.unit.DAY, 360);
    }
     
    out.println(cacheToFile.get("your key"));
    out.println("From not cache");
    }
