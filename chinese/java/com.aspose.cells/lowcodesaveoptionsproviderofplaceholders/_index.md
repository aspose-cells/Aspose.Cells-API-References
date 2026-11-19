---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells for Java API 参考"
description: "实现提供保存选项，将拆分部分保存为文件，生成文件的路径使用占位符定义。"
type: docs
url: /zh/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

实现提供保存选项，将拆分部分保存为文件，生成文件的路径使用占位符定义。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | 实例化一个对象，以根据指定的模板提供保存选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | 在处理当前拆分部分后释放资源。 |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | 是否始终在文件路径中添加工作表索引或名称。 |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | 是否始终在文件路径中添加拆分部分索引。 |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | 获取用于获取当前拆分部分输出设置的保存选项。 |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | 用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。 |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | 文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。 |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | 工作表索引的前缀。 |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | 工作表索引的前缀。 |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | 文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。 |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | 拆分部分索引的前缀。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | 是否始终在文件路径中添加工作表索引或名称。 |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | 是否始终在文件路径中添加拆分部分索引。 |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | 用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。 |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | 文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。 |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | 工作表索引的前缀。 |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | 工作表索引的前缀。 |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | 文件路径中使用的拆分部分索引与其实际值之间的偏移量（[SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)）。 |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | 拆分部分索引的前缀。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


实例化一个对象，以根据指定的模板提供保存选项。

**Remarks**

文件路径模板中支持的占位符：

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pathTemplate | java.lang.String | 生成的文件路径的模板。 |

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


是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引和名称以及相应的前缀（[getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)）不会添加到文件路径中。

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


是否始终在文件路径中添加拆分部分索引。默认值为 false，即当只有一个拆分部分时，拆分部分索引以及相应的前缀（[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)）不会添加到文件路径中。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。

**Remarks**

如果已指定模板，则创建的实例将复制其中的所有设置并相应地更新输出文件。

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


文件路径中使用的工作表索引与其实际值之间的偏移量（[SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)）。

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) 为 false，则此前缀以及工作表索引（或名称）将不会添加到生成的文件路径中。

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) 为 false，则此前缀以及工作表索引（或名称）将不会添加到生成的文件路径中。

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

如果只有一个拆分部分且 [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) 为 false，则此前缀以及拆分部分索引（0）将不会添加到生成的文件路径中。

**Returns:**
java.lang.String
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


是否始终在文件路径中添加工作表索引或名称。默认值为 false，即当只有一个工作表时，工作表索引和名称以及相应的前缀（[getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)）不会添加到文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


是否始终在文件路径中添加拆分部分索引。默认值为 false，即当只有一个拆分部分时，拆分部分索引以及相应的前缀（[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)）不会添加到文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


用于在 [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-) 中创建保存选项实例的模板。

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

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) 为 false，则此前缀以及工作表索引（或名称）将不会添加到生成的文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


工作表索引的前缀。

**Remarks**

如果只有一个工作表且 [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) 为 false，则此前缀以及工作表索引（或名称）将不会添加到生成的文件路径中。

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

如果只有一个拆分部分且 [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) 为 false，则此前缀以及拆分部分索引（0）将不会添加到生成的文件路径中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

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

