---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells for Java API 参考"
description: "实现提供保存选项，以将拆分部分保存到文件，并且生成文件的路径命名方式可能包含目录 SheetIndex 或 SheetName SplitPartIndex。"
type: docs
url: /zh/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

实现提供保存选项，以将拆分部分保存到文件，并且生成文件的路径命名方式为（可能包含目录）：[getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(or SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | 在处理当前拆分部分后释放资源。 |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | 是否始终在文件路径中添加工作表索引或名称。 |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | 是否始终在文件路径中添加拆分部分索引。 |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | 文件路径的头部（在添加工作表和拆分部分内容之前）。 |
| [getPathTail()](#getPathTail--) | 文件路径的尾部（在序列号之后）。 |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | 获取用于获取当前拆分部分输出设置的保存选项。 |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | 用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。 |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | 文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。 |
| [getSheetPrefix()](#getSheetPrefix--) | 工作表索引的前缀。 |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | 文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。 |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | 拆分部分索引的前缀。 |
| [getUseSheetName()](#getUseSheetName--) | 是否使用工作表名称而非工作表索引构建文件路径。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | 是否始终在文件路径中添加工作表索引或名称。 |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | 是否始终在文件路径中添加拆分部分索引。 |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | 文件路径的头部（在添加工作表和拆分部分内容之前）。 |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | 文件路径的尾部（在序列号之后）。 |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | 用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。 |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | 文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。 |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | 工作表索引的前缀。 |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | 文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。 |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | 拆分部分索引的前缀。 |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | 是否使用工作表名称而非工作表索引构建文件路径。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
```


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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


在处理当前拆分部分后释放资源。

**Remarks**

默认情况下，此方法直接关闭由[LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)指定的流（如果保存选项将流作为目标）。用户可以覆盖此方法，以根据其需求以及[getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-)的实现来控制资源的释放方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | 用于当前拆分部分的保存选项。 |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀将不会添加到文件路径中。

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


是否始终在文件路径中添加拆分部分索引。默认值为 false，即当只有一个拆分部分时，拆分部分索引及相应前缀将不会添加到文件路径中。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


文件路径的头部（在添加工作表和拆分部分内容之前）。

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


文件路径的尾部（在序列号之后）。它应包括文件名的扩展名。

**Returns:**
java.lang.String
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


获取用于获取当前拆分部分输出设置的保存选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。

**Remarks**

如果已指定模板，则创建的实例将复制其中的所有设置并相应地更新输出文件。

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。

**Remarks**

仅在 [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) 为 false 时生效。

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) 为 false，则此前缀和工作表索引（或名称）将不会添加到生成的文件路径中。

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


拆分部分索引的前缀。

**Remarks**

如果只有一个拆分部分且 [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) 为 false，则此前缀和拆分部分索引（0）将不会添加到生成的文件路径中。

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


是否使用工作表名称而非工作表索引来构建文件路径。默认值为 false。

**Remarks**

工作表名称永远不会自动重新构建。因此当将其设置为 true 时，请确保没有可能导致文件路径或名称无效的特殊工作表名称。

**Returns:**
boolean
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀将不会添加到文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


是否始终在文件路径中添加拆分部分索引。默认值为 false，即当只有一个拆分部分时，拆分部分索引及相应前缀将不会添加到文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


文件路径的头部（在添加工作表和拆分部分内容之前）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


文件路径的尾部（在序列号之后）。它应包括文件名的扩展名。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。

**Remarks**

如果已指定模板，则创建的实例将复制其中的所有设置并相应地更新输出文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。

**Remarks**

仅在 [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) 为 false 时生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) 为 false，则此前缀和工作表索引（或名称）将不会添加到生成的文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


拆分部分索引的前缀。

**Remarks**

如果只有一个拆分部分且 [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) 为 false，则此前缀和拆分部分索引（0）将不会添加到生成的文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


是否使用工作表名称而非工作表索引来构建文件路径。默认值为 false。

**Remarks**

工作表名称永远不会自动重新构建。因此当将其设置为 true 时，请确保没有可能导致文件路径或名称无效的特殊工作表名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

