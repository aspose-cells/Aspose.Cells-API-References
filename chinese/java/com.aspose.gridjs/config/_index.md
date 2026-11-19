---
title: "Config"
second_title: "Aspose.Cells for Java API 参考"
description: "表示 GridJs 的所有静态设置"
type: docs
url: /zh/java/com.aspose.gridjs/config/
---

**Inheritance:**
java.lang.Object
```
public class Config
```

表示 GridJs 的所有静态设置
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Config()](#Config--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
| [RedactionUseClientGenerateId](#RedactionUseClientGenerateId) | 指示在与编辑相关的操作中是否使用客户端生成的 ID 而非实际的形状 ID |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitColumnsOnLoad()](#getAutoFitColumnsOnLoad--) | 指示在文件加载期间是否自动调整列宽。 |
| [getAutoFitRowsHeightOnLoad()](#getAutoFitRowsHeightOnLoad--) | 指示在文件加载期间是否自动调整行高。 |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | 获取是否自动优化具有大单元格的工作表的加载性能。 |
| [getBaseRouteName()](#getBaseRouteName--) | 获取 GridJs 控制器 URL 的基础路由名称。默认值为 "/GridJs2"。 |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | 获取空工作表的默认最大列数。 |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | 获取空工作表的默认最大行数。 |
| [getEnableChartClientRendering()](#getEnableChartClientRendering--) | 获取是否启用客户端图表渲染。 |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | 获取用于存储电子表格文件的缓存目录。 |
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
| [setAutoFitColumnsOnLoad(boolean value)](#setAutoFitColumnsOnLoad-boolean-) | 指示在文件加载期间是否自动调整列宽。 |
| [setAutoFitRowsHeightOnLoad(boolean value)](#setAutoFitRowsHeightOnLoad-boolean-) | 指示在文件加载期间是否自动调整行高。 |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | 设置是否自动优化大单元格工作表的加载性能。 |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | 设置 GridJs 控制器 URL 的基础路由名称。默认值为 "/GridJs2"。 |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | 设置是否支持协作编辑，默认值为 false。 |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | 设置空工作表的默认最大列数。 |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | 设置空工作表的默认最大行数。 |
| [setEnableChartClientRendering(boolean value)](#setEnableChartClientRendering-boolean-) | 设置是否启用客户端图表渲染。 |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | 设置用于存储电子表格文件的缓存目录。 |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | 设置字体文件夹 |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | 设置字体文件夹 |
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
### Config() {#Config--}
```
public Config()
```


### RedactionUseClientGenerateId {#RedactionUseClientGenerateId}
```
public static boolean RedactionUseClientGenerateId
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
public static boolean getAutoFitColumnsOnLoad()
```


指示在文件加载期间是否自动调整列宽。默认值为 `false`。警告：将其设置为 `true` 将在加载后执行所有列的自动调整操作，这可能对性能产生显著影响。

**Returns:**
boolean
### getAutoFitRowsHeightOnLoad() {#getAutoFitRowsHeightOnLoad--}
```
public static boolean getAutoFitRowsHeightOnLoad()
```


指示在文件加载期间是否自动调整行高。默认值为 `false`。警告：将其设置为 `true` 将在加载后执行所有行的自动调整操作，这可能对性能产生显著影响。

**Returns:**
boolean
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```


获取是否自动优化大单元格工作表的加载性能。它将忽略某些样式/边框以减少加载时间，默认值为 true。

**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```


获取 GridJs 控制器 URL 的基础路由名称。默认值为 "/GridJs2"。

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
public static int getEmptySheetMaxCol()
```


获取空工作表的默认最大列数，默认值为 15。

**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```


获取空工作表的默认最大行数，默认值为 12。

**Returns:**
int
### getEnableChartClientRendering() {#getEnableChartClientRendering--}
```
public static boolean getEnableChartClientRendering()
```


获取是否启用客户端图表渲染。如果设置为 false，GridJs 将仅回退到服务器生成的图表图像/形状。默认值为 true。

**Returns:**
boolean
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```


获取用于存储电子表格文件的缓存目录。在使用 GridJs 之前，我们需要将其设置为特定路径。

**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```


获取是否显示包含数据、样式、合并单元格和形状的最大范围。如果最后一行或列包含没有值和公式但具有自定义样式的单元格，则在此值为 true 时我们将不显示该行/列。\u9286?\* 默认值为 true。

**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```


获取是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。

**Returns:**
boolean
### getJsonCache() {#getJsonCache--}
```
public static JsonCacheOptions getJsonCache()
```


获取 JSON 缓存配置选项。控制生成的工作簿 JSON 的内存 (L1) 和磁盘 (L2) 缓存行为。

**Returns:**
[JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions)
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```


获取是否仅加载活动工作表，默认值为 false。

**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```


获取保存为 PDF 时的最大超时时间（秒）。默认值为 10。

**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```


获取活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 100。

**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```


获取形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。默认值为 10000。

**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```


获取工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 300。

**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```


获取以 "/topic" 为前缀的 WebSocket 目标地址，默认是 "/topic/opr"，仅在协作模式下使用。

**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```


获取图片的缓存目录。（当 GridJsWorkbook.CacheImp 为 null 时生效）默认路径为 FileCacheDirectory 中的 "\_piccache"。

**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```


获取是否检查图像是否具有相同来源，默认值为 true。

**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```


获取是否将 HTML 文件保存为 zip 压缩包，默认值为 false。

**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```


获取是否显示图表工作表。默认值为 false。

**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```


获取是否跳过对 UI 不可见的形状，默认值为 true。

**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
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
public static boolean isCollaborative()
```


获取是否支持协作编辑，默认值为 false。

**Returns:**
boolean
### isWasm() {#isWasm--}
```
public static boolean isWasm()
```


获取 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。当为 true 时，不使用 FileCacheDirectory / 磁盘 / 中断线程路径，文件缓存必须来自 GridJsOptions.CacheImp。GridJsOptions.IsWasm 在构建 GridJs 服务时设置此项，因此一个 Aspose.Cells.GridJs.dll 可同时服务两种主机。默认值为 false。

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
public static void setAutoFitColumnsOnLoad(boolean value)
```


指示在文件加载期间是否自动调整列宽。默认值为 `false`。警告：将其设置为 `true` 将在加载后执行所有列的自动调整操作，这可能对性能产生显著影响。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoFitRowsHeightOnLoad(boolean value) {#setAutoFitRowsHeightOnLoad-boolean-}
```
public static void setAutoFitRowsHeightOnLoad(boolean value)
```


指示在文件加载期间是否自动调整行高。默认值为 `false`。警告：将其设置为 `true` 将在加载后执行所有行的自动调整操作，这可能对性能产生显著影响。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```


设置是否自动优化包含大单元格的工作表的加载性能。它将忽略某些样式/边框以减少加载时间。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```


设置 GridJs 控制器 URL 的基础路由名称。默认值为 "/GridJs2"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```


设置是否支持协作编辑，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```


设置空工作表的默认最大列数。默认值为 15。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```


设置空工作表的默认最大行数。默认值为 12。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnableChartClientRendering(boolean value) {#setEnableChartClientRendering-boolean-}
```
public static void setEnableChartClientRendering(boolean value)
```


设置是否启用客户端图表渲染。如果设置为 false，GridJs 将仅回退到服务器生成的图表图像/形状。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```


设置用于存储电子表格文件的缓存目录。我们需要在使用 GridJs 之前将其设置为特定路径。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolder | java.lang.String | 包含 TrueType 字体的文件夹。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


设置字体文件夹

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFolders | java.lang.String[] | 包含 TrueType 字体的文件夹集合。 |
| recursive | boolean | 确定是否扫描子文件夹。 |

### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```


设置是否显示包含数据、样式、合并单元格和形状的最大范围。如果最后一行或列包含没有值和公式但具有自定义样式的单元格，则在此值为 true 时我们将不显示该行/列。\u9286?\* 默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```


设置是否限制单个工作表中显示的形状/图像总数；如果设置为 true，GridJs 将把单个工作表中显示的形状或图像的总数限制为 MaxShapeOrImageCount，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setJsonCache(JsonCacheOptions value) {#setJsonCache-com.aspose.gridjs.JsonCacheOptions-}
```
public static void setJsonCache(JsonCacheOptions value)
```


设置 JSON 缓存配置选项。控制生成的工作簿 JSON 的内存 (L1) 和磁盘 (L2) 缓存行为。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [JsonCacheOptions](../../com.aspose.gridjs/jsoncacheoptions) |  |

### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```


设置是否仅加载活动工作表，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```


设置保存为 PDF 时的最大超时时间（秒）。默认值为 10。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```


设置活动工作表中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```


设置形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，仅在 IslimitShapeOrImage=true 时生效。默认值为 10000。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```


设置工作簿中显示的形状或图像的总数，仅在 IslimitShapeOrImage=true 时生效。默认值为 300。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```


设置以 "/topic" 为前缀的 WebSocket 目标，默认是 "/topic/opr"，仅在协作模式下使用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```


设置图片的缓存目录。（当 GridJsWorkbook.CacheImp 为 null 时生效）默认路径为 FileCacheDirectory 中的 "\_piccache"。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```


设置是否检查图像是否具有相同来源，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```


设置是否将 HTML 文件保存为 zip 压缩包，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```


设置是否显示图表工作表。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```


设置是否跳过对 UI 不可见的形状，默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```


设置在工作表具有 PageSetup 打印区域设置时，是否在 UI 显示范围中使用 PageSetup.PrintArea。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWasm(boolean value) {#setWasm-boolean-}
```
public static void setWasm(boolean value)
```


设置 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中运行。为 true 时，不使用 FileCacheDirectory / 磁盘 / 中断线程路径，文件缓存必须来自 GridJsOptions.CacheImp。GridJsOptions.IsWasm 在构建 GridJs 服务时设置此项，因此一个 Aspose.Cells.GridJs.dll 可同时服务于两种主机。默认值为 false。

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

