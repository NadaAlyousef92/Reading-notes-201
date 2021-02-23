# **THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS**

* Persistent local storage is one of the areas where native client applications have held an advantage over web applications*

What we develpers want is:

*a lot of storage spaceon the clientthat persists beyond a page refreshand isn’t transmitted to the server
Before HTML5, all attempts to chieve this were ultimately unsatisfactory in different ways.**

## INTRODUCING HTML5 STORAGE

***“HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.***
***“Local Storage” or “DOM Storage.” The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.***

### **USING HTML5 STORAGE**

- You store data based on a named key,HTML5 Storage is based on named key/value pairs.then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.
- There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).
  Calling removeItem() with a non-existent key will do nothing.
- Finally there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index to get the name of each key.

|STORAGEEVENT OBJECT|
|---------|-----|------|-------------|
|PROPERTY|TYPE|DESCRIPTION|
|key     |string| the named key that was added, removed, or modified|
|oldValue|any|the previous value (now overwritten), or null if a new item was added|
|newValue|any|the new value, or null if an item was removed|
|url*    |string|the page which called a method that triggered this change|
|* Note: the url property was originally called uri. Some browsers shipped with that property before the specification changed. For maximum compatibility, you should check whether the url property exists, and if not, check for the uri property instead.|

#### **LIMITATIONS IN CURRENT BROWSERS**

**“5 megabytes” is how much storage space each origin gets by default. This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification.**

[link](!https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.exeideas.com%2F2016%2F03%2Fhtml5-local-storage.html&psig=AOvVaw1DttYMbZEJZwBQ59jgBL3O&ust=1614135644782000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCIj46oiC_-4CFQAAAAAdAAAAABAD)

[link](http://diveinto.html5doctor.com/storage.html)