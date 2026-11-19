---
title: "StreamProviderOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示流选项。"
type: docs
url: /zh/java/com.aspose.cells/streamprovideroptions/
---

**Inheritance:**
java.lang.Object
```
public class StreamProviderOptions
```

表示流选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [StreamProviderOptions(int loadingType, String defaultPath)](#StreamProviderOptions-int-java.lang.String-) | 初始化 [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) 类的新实例。 |
| [StreamProviderOptions()](#StreamProviderOptions--) | 初始化 [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomPath()](#getCustomPath--) | 用户自定义路径（URL）已保存到生成的 html 文件中，用于引用的源。 |
| [getDefaultPath()](#getDefaultPath--) | 默认路径（URL）已保存到生成的 html 文件中，用于引用的源。 |
| [getInputStream()](#getInputStream--) | 获取输入流以获取数据。 |
| [getResourceLoadingType()](#getResourceLoadingType--) | 获取加载资源的类型。 |
| [getStream()](#getStream--) | 获取输出流以写入已保存的数据。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomPath(String value)](#setCustomPath-java.lang.String-) | 用户自定义路径（URL）已保存到生成的 html 文件中，用于引用的源。 |
| [setInputStream(InputStream value)](#setInputStream-java.io.InputStream-) | 设置用于获取数据的输入流。 |
| [setResourceLoadingType(int value)](#setResourceLoadingType-int-) | 设置加载资源的类型。 |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | 设置输出流以写入已保存的数据。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StreamProviderOptions(int loadingType, String defaultPath) {#StreamProviderOptions-int-java.lang.String-}
```
public StreamProviderOptions(int loadingType, String defaultPath)
```


初始化 [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loadingType | int | [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype)。用于加载链接资源的类型。 |
| defaultPath | java.lang.String | 默认路径。 |

### StreamProviderOptions() {#StreamProviderOptions--}
```
public StreamProviderOptions()
```


初始化 [StreamProviderOptions](../../com.aspose.cells/streamprovideroptions) 类的新实例。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
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
### getCustomPath() {#getCustomPath--}
```
public String getCustomPath()
```


用户自定义路径（URL）已保存到生成的 html 文件中，用于引用的源。如果用户未定义，将使用 DefaultPath。例如，工作表数据将由用户保存到 d:/sheet001.htm，主 html 文件中使用的 url 应为 "d:/sheet001.htm" 或其他可被主 html 文件访问的有效相对路径。

**Returns:**
java.lang.String
### getDefaultPath() {#getDefaultPath--}
```
public String getDefaultPath()
```


默认路径（URL）已保存到生成的 html 文件中，用于引用的源。例如，工作表数据保存在 xxx\_files/sheet001.htm，主 html 文件中使用的 url 应类似于 "src=\"xxx\_files/sheet001.htm\""。

**Returns:**
java.lang.String
### getInputStream() {#getInputStream--}
```
public InputStream getInputStream()
```


获取输入流以获取数据。

**Returns:**
java.io.InputStream
### getResourceLoadingType() {#getResourceLoadingType--}
```
public int getResourceLoadingType()
```


获取加载资源的类型。

参见 [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype)。

**Returns:**
int
### getStream() {#getStream--}
```
public OutputStream getStream()
```


获取输出流以写入已保存的数据。

**Returns:**
java.io.OutputStream
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCustomPath(String value) {#setCustomPath-java.lang.String-}
```
public void setCustomPath(String value)
```


用户自定义路径（URL）已保存到生成的 html 文件中，用于引用的源。如果用户未定义，将使用 DefaultPath。例如，工作表数据将由用户保存到 d:/sheet001.htm，主 html 文件中使用的 url 应为 "d:/sheet001.htm" 或其他可被主 html 文件访问的有效相对路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setInputStream(InputStream value) {#setInputStream-java.io.InputStream-}
```
public void setInputStream(InputStream value)
```


设置用于获取数据的输入流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.io.InputStream |  |

### setResourceLoadingType(int value) {#setResourceLoadingType-int-}
```
public void setResourceLoadingType(int value)
```


设置加载资源的类型。

参见 [ResourceLoadingType](../../com.aspose.cells/resourceloadingtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public void setStream(OutputStream value)
```


设置输出流以写入已保存的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.io.OutputStream |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

