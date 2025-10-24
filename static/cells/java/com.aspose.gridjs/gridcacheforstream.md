##GridCacheForStream
This class contains the cache operations for GridJs.
**Inheritance:**
java.lang.Object
```
public abstract class GridCacheForStream
```
This class contains the cache operations for GridJs. User shall implement his own business logic for storage based on it..
## Constructors
| Constructor | Description |
| --- | --- |
| [GridCacheForStream()](#GridCacheForStream--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFileUrl(String uid)](#getFileUrl-java.lang.String-) | Implements this method to get the file url from the cache. |
| [hashCode()](#hashCode--) |  |
| [isExisted(String uid)](#isExisted-java.lang.String-) | Checks whether the cache with uid is existed |
| [loadStream(String uid)](#loadStream-java.lang.String-) | Implements this method to load cache with the key uid,return the stream from the cache. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveStream(InputStream s, String uid)](#saveStream-java.io.InputStream-java.lang.String-) | Implements this method to save cache,save the stream to the cache with the key uid. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridCacheForStream() {#GridCacheForStream--}
```
public GridCacheForStream()
```
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFileUrl(String uid) {#getFileUrl-java.lang.String-}
```
public abstract String getFileUrl(String uid)
```
Implements this method to get the file url from the cache.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
**Returns:**
java.lang.String - The URL of the file
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isExisted(String uid) {#isExisted-java.lang.String-}
```
public abstract boolean isExisted(String uid)
```
Checks whether the cache with uid is existed
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String | The unique id for the file cache. |
**Returns:**
boolean - The bool value
### loadStream(String uid) {#loadStream-java.lang.String-}
```
public abstract InputStream loadStream(String uid)
```
Implements this method to load cache with the key uid,return the stream from the cache.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | java.lang.String |  |
**Returns:**
java.io.InputStream
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### saveStream(InputStream s, String uid) {#saveStream-java.io.InputStream-java.lang.String-}
```
public abstract void saveStream(InputStream s, String uid)
```
Implements this method to save cache,save the stream to the cache with the key uid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |
| uid | java.lang.String |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
