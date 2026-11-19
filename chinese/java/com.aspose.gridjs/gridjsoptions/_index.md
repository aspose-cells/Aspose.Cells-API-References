---
title: "GridJsOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 GridJs 的所有加载选项"
type: docs
url: /zh/java/com.aspose.gridjs/gridjsoptions/
---

**Inheritance:**
java.lang.Object
```
public class GridJsOptions
```

表示 GridJs 的所有加载选项
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridJsOptions()](#GridJsOptions--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
| [CacheImp](#CacheImp) | 用于缓存存储的自定义实现，如果您想以流方式存储缓存，需要进行设置和实现。 |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | 指示在与编辑相关的操作中是否使用客户端生成的 ID 而非实际的形状 ID |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | 指示在加载文件时是否自动调整列宽，默认值为 false。 |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | 指示在加载文件时是否自动调整行高，默认值为 false。 |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | 获取是否自动优化具有大单元格的工作表的加载性能。 |
| [getBaseRouteName()](#getBaseRouteName--) | 获取 GridJs 控制器的路由 URL 基础名称，默认是 GridJs2。 |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | 获取空工作表的默认最大列数。 |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | 获取空工作表的默认最大行数。 |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | 获取是否启用客户端图表渲染。 |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | 获取用于存储电子表格文件的缓存目录。 |
| [getFontFolders()](#getFontFolders--) | 获取渲染图片/形状中字体的字体文件夹。 |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | 获取是否显示包含数据、样式、合并单元格和形状的最大范围。 |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | 获取是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。 |
| [getJsonCache()](#getJsonCache--) | 获取 JSON 缓存配置选项。 |
| [getLazyLoading()](#getLazyLoading--) | 获取是否仅加载活动工作表，默认值为 false。 |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | 获取保存为 PDF 时的最大超时时间（秒）。 |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | 获取活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。 |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | 获取形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。 |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | 获取工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。 |
| [getMessageTopic()](#getMessageTopic--) | 获取以 "/topic" 为前缀的 WebSocket 目标地址，默认是 "/topic/opr"，仅在协作模式下使用。 |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | 获取图片的缓存目录。 |
| [getSameImageDetecting()](#getSameImageDetecting--) | 获取是否检查图像是否具有相同来源，默认值为 true。 |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | 获取是否将 HTML 文件保存为 zip 压缩包，默认值为 false。 |
| [getShowChartSheet()](#getShowChartSheet--) | 获取是否显示图表工作表。 |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | 获取是否跳过对 UI 不可见的形状，默认值为 true。 |
| [getUsePrintArea()](#getUsePrintArea--) | 获取在工作表具有 PageSetup 打印区域设置时，是否使用 PageSetup.PrintArea 作为 UI 显示范围。 |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | 获取是否支持协作编辑，默认值为 false。 |
| [isWasm()](#isWasm--) | 获取 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | 指示在加载文件时是否自动调整列宽，默认值为 false。 |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | 指示在加载文件时是否自动调整行高，默认值为 false。 |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | 设置是否自动优化大单元格工作表的加载性能。 |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | 设置 GridJs 控制器的路由 URL 基础名称，默认是 GridJs2。 |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | 设置是否支持协作编辑，默认值为 false。 |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | 设置空工作表的默认最大列数。 |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | 设置空工作表的默认最大行数。 |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | 设置是否启用客户端图表渲染。 |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | 设置用于存储电子表格文件的缓存目录。 |
| [setFontFolders(String[] value)](#setFontFolders-java.lang.String---) | 设置渲染图片/形状中字体的字体文件夹。 |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | 设置是否显示包含数据、样式、合并单元格和形状的最大范围。 |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | 设置是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。 |
| [setJsonCache(JsonCacheOptions value)](#setJsonCache-com.aspose.gridjs.JsonCacheOptions-) | 设置 JSON 缓存配置选项。 |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | 设置是否仅加载活动工作表，默认值为 false。 |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | 设置保存为 PDF 时的最大超时时间（秒）。 |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | 设置活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。 |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | 设置形状或图像的最大宽度或高度；GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。 |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | 设置工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。 |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | 设置以 "/topic" 为前缀的 WebSocket 目标，默认是 "/topic/opr"，仅在协作模式下使用。 |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | 设置图片的缓存目录。 |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | 设置是否检查图像是否具有相同来源，默认值为 true。 |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | 设置是否将 HTML 文件保存为 zip 压缩包，默认值为 false。 |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | 设置是否显示图表工作表。 |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | 设置是否跳过对 UI 不可见的形状，默认值为 true。 |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | 设置在工作表具有 PageSetup 打印区域设置时，是否使用 PageSetup.PrintArea 作为 UI 显示范围。 |
| [setWasm(boolean value)](#setWasm-boolean-) | 设置 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridJsOptions() {#GridJsOptions--}
```
public GridJsOptions()
```


### CacheImp {#CacheImp}
```
public GridCacheForStream CacheImp
```


缓存存储的自定义实现；如果您想以流方式存储缓存，需要进行设置和实现。WebAssembly 主机（IsWasm = true）必须设置它，因为默认文件缓存没有本地磁盘。

### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public boolean RedactionUseClientGenerateId
```


指示在与编辑相关的操作中是否使用客户端生成的 ID 而非实际的形状 ID

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
### getAutoFitColumnsOnLoad() {#getAutoFitColumnsOnLoad--}
```
public boolean getAutoFitColumnsOnLoad()
```


指示在加载文件时是否自动调整列宽，默认值为 false。

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public boolean getAutoFitRowsHeightOnLoad()
```


指示在加载文件时是否自动调整行高，默认值为 false。

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public boolean getAutoOptimizeForLargeCells()
```


获取是否自动优化大单元格工作表的加载性能。它将忽略某些样式/边框以减少加载时间，默认值为 true。

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public String getBaseRouteName()
```


获取 GridJs 控制器的路由 URL 基础名称，默认是 GridJs2。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmptySheetMaxCol() {#getEmptySheetMaxCol--}
```
public int getEmptySheetMaxCol()
```


获取空工作表的默认最大列数，默认值为 15。

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public int getEmptySheetMaxRow()
```


获取空工作表的默认最大行数，默认值为 12。

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public boolean getEnableChartClientRendering()
```


获取是否启用客户端图表渲染。如果设置为 false，GridJs 将仅生成图表图像/形状，不需要客户端图表渲染，默认值为 true。

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public String getFileCacheDirectory()
```


获取用于存储电子表格文件的缓存目录。在使用 GridJs 之前，我们需要将其设置为特定路径。

**Returns:**
java.lang.String
### getFontFolders() {#getFontFolders--}
```
public String[] getFontFolders()
```


获取渲染图片/形状中字体的字体文件夹。

**Returns:**
java.lang.String[]
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public boolean getIgnoreEmptyContent()
```


获取是否显示包含数据、样式、合并单元格和形状的最大范围。如果最后一行或列包含没有值和公式但具有自定义样式的单元格，则在此值为 true 时我们将不显示该行/列。\u9286?\* 默认值为 true。

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public boolean getIslimitShapeOrImage()
```


获取是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public JsonCacheOptions getJsonCache()
```


获取 JSON 缓存配置选项。控制生成的工作簿 JSON 的内存 (L1) 和磁盘 (L2) 缓存行为。

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public boolean getLazyLoading()
```


获取是否仅加载活动工作表，默认值为 false。

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public int getMaxPdfSaveSeconds()
```


获取保存为 PDF 时的最大超时时间（秒）。默认值为 10。

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public int getMaxShapeOrImageCount()
```


获取活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 100。

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public int getMaxShapeOrImageWidthOrHeight()
```


获取形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。默认值为 10000。

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public int getMaxTotalShapeOrImageCount()
```


获取工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 300。

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public String getMessageTopic()
```


获取以 "/topic" 为前缀的 WebSocket 目标地址，默认是 "/topic/opr"，仅在协作模式下使用。

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public String getPictureCacheDirectory()
```


获取图片的缓存目录。（当 GridJsWorkbook.CacheImp 为 null 时生效）默认路径为 FileCacheDirectory 中的 "\_piccache"。

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public boolean getSameImageDetecting()
```


获取是否检查图像是否具有相同来源，默认值为 true。

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public boolean getSaveHtmlAsZip()
```


获取是否将 HTML 文件保存为 zip 压缩包，默认值为 false。

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public boolean getShowChartSheet()
```


获取是否显示图表工作表。默认值为 false。

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public boolean getSkipInvisibleShapes()
```


获取是否跳过对 UI 不可见的形状，默认值为 true。

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public boolean getUsePrintArea()
```


获取在工作表具有 PageSetup 打印区域设置时，是否在 UI 显示范围中使用 PageSetup.PrintArea。默认值为 false。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCollaborative() {#isCollaborative--}
```
public boolean isCollaborative()
```


获取是否支持协作编辑，默认值为 false。

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public boolean isWasm()
```


获取 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。为 true 时，不使用 FileCacheDirectory / 磁盘 / 中断线程路径，文件缓存必须来自 CacheImp，因为浏览器主机没有本地磁盘。它在运行时选择代码路径，因此一个 Aspose.Cells.GridJs.dll 可服务于两种主机。默认值为 false。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoFitColumnsOnLoad(boolean value) {#setAutoFitColumnsOnLoad-boolean-}
```
public void setAutoFitColumnsOnLoad(boolean value)
```


指示在加载文件时是否自动调整列宽，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public void setAutoFitRowsHeightOnLoad(boolean value)
```


指示在加载文件时是否自动调整行高，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public void setAutoOptimizeForLargeCells(boolean value)
```


设置是否自动优化包含大单元格的工作表的加载性能。它将忽略某些样式/边框以减少加载时间。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public void setBaseRouteName(String value)
```


设置 GridJs 控制器的路由 URL 基础名称，默认是 GridJs2。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public void setCollaborative(boolean value)
```


设置是否支持协作编辑，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public void setEmptySheetMaxCol(int value)
```


设置空工作表的默认最大列数。默认值为 15。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public void setEmptySheetMaxRow(int value)
```


设置空工作表的默认最大行数。默认值为 12。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public void setEnableChartClientRendering(boolean value)
```


设置是否启用客户端图表渲染。如果设为 false，GridJs 将仅输出图表图像/形状，不需要客户端图表渲染。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public void setFileCacheDirectory(String value)
```


设置用于存储电子表格文件的缓存目录。我们需要在使用 GridJs 之前将其设置为特定路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFontFolders(String[] value) {#setFontFolders-java.lang.String---}
```
public void setFontFolders(String[] value)
```


设置渲染图片/形状中字体的字体文件夹。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String[] |  |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public void setIgnoreEmptyContent(boolean value)
```


设置是否显示包含数据、样式、合并单元格和形状的最大范围。如果最后一行或列包含没有值和公式但具有自定义样式的单元格，则在此值为 true 时我们将不显示该行/列。\u9286?\* 默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public void setIslimitShapeOrImage(boolean value)
```


设置是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public void setJsonCache(JsonCacheOptions value)
```


设置 JSON 缓存配置选项。控制生成的工作簿 JSON 的内存 (L1) 和磁盘 (L2) 缓存行为。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public void setLazyLoading(boolean value)
```


设置是否仅加载活动工作表，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public void setMaxPdfSaveSeconds(int value)
```


设置保存为 PDF 时的最大超时时间（秒）。默认值为 10。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public void setMaxShapeOrImageCount(int value)
```


设置活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public void setMaxShapeOrImageWidthOrHeight(int value)
```


设置形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。默认值为 10000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public void setMaxTotalShapeOrImageCount(int value)
```


设置工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 300。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public void setMessageTopic(String value)
```


设置以 "/topic" 为前缀的 WebSocket 目标，默认是 "/topic/opr"，仅在协作模式下使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public void setPictureCacheDirectory(String value)
```


设置图片的缓存目录。（当 GridJsWorkbook.CacheImp 为 null 时生效）默认路径为 FileCacheDirectory 中的 "\_piccache"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public void setSameImageDetecting(boolean value)
```


设置是否检查图像是否具有相同来源，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public void setSaveHtmlAsZip(boolean value)
```


设置是否将 HTML 文件保存为 zip 压缩包，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public void setShowChartSheet(boolean value)
```


设置是否显示图表工作表。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public void setSkipInvisibleShapes(boolean value)
```


设置是否跳过对 UI 不可见的形状，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public void setUsePrintArea(boolean value)
```


设置在工作表具有 PageSetup 打印区域设置时，是否在 UI 显示范围中使用 PageSetup.PrintArea。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public void setWasm(boolean value)
```


设置 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。为 true 时，不使用 FileCacheDirectory / 磁盘 / 中断线程路径，文件缓存必须来自 CacheImp，因为浏览器主机没有本地磁盘。它在运行时选择代码路径，因此一个 Aspose.Cells.GridJs.dll 可服务于两种主机。默认值为 false。

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

