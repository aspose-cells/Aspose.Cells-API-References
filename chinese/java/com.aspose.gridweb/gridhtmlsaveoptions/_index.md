---
title: "GridHtmlSaveOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示保存 HTML 文件的选项。"
type: docs
url: /zh/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object，[com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

表示保存 HTML 文件的选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | 创建用于保存 html 文件的选项。 |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | 创建用于保存 htm 文件的选项。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | 附件文件将保存到的目录。 |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | 指定 html 文件中附加文件（如图像）的 Url 前缀。 |
| [getCachedFileFolder()](#getCachedFileFolder--) | 缓存文件夹用于存储一些大数据。 |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | 在保存文件后使工作簿为空。 |
| [getCreateDirectory()](#getCreateDirectory--) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [getDefaultFontName()](#getDefaultFontName--) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。 |
| [getEncoding()](#getEncoding--) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | 指示是否将整个工作簿导出为 HTML 文件。 |
| [getExportArea()](#getExportArea--) | 获取当前活动工作表的导出 CellArea。 |
| [getExportGridLines()](#getExportGridLines--) | 指示是否导出网格线。默认值为 false。 |
| [getExportHeadings()](#getExportHeadings--) | 指示在保存文件为 HTML 时是否导出标题。默认值为 false。 |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | 指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | 指示是否仅将打印区域导出为 HTML 文件。 |
| [getExportSingleTab()](#getExportSingleTab--) | 指示当文件只有一个工作表时是否导出单个标签页。 |
| [getMergeAreas()](#getMergeAreas--) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [getPageTitle()](#getPageTitle--) | HTML 页面标题。 |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | 解析单元格中的 HTML 标签，例如 |

,作为单元格值，或作为 html 标签，默认是 true |
| [getPresentationPreference()](#getPresentationPreference--) | 指示 html 或 mht 文件是否为呈现首选项。默认值为 false。如果您想获得更美观的呈现，请将该值设置为 true。 |
| [getRefreshChartCache()](#getRefreshChartCache--) | 指示是否刷新图表缓存数据 |
| [getSaveFormat()](#getSaveFormat--) | 获取保存的文件格式。 |
| [getSortNames()](#getSortNames--) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | 指示在保存文件之前是否验证合并的单元格。 |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | 指示在将文件保存为 HTML 时是否导出注释，默认值为 false。 |
| [isFullPathLink()](#isFullPathLink--) | 指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | 附件文件将保存到的目录。 |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | 指定 html 文件中附加文件（如图像）的 Url 前缀。 |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | 缓存文件夹用于存储一些大数据。 |
| [setClearData(boolean value)](#setClearData-boolean-) | 在保存文件后使工作簿为空。 |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | 指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。 |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | 如果未设置，则使用 Encoding.UTF8 作为默认编码类型。 |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | 指示是否将整个工作簿导出为 HTML 文件。 |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | 设置当前活动工作表的导出 CellArea。 |
| [setExportComments(boolean value)](#setExportComments-boolean-) | 指示在将文件保存为 HTML 时是否导出注释，默认值为 false。 |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | 指示是否导出网格线。默认值为 false。 |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | 指示在保存文件为 HTML 时是否导出标题。默认值为 false。 |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | 指示是否导出隐藏工作表的内容。默认值为 true。 |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | 指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。 |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | 指示是否仅将打印区域导出为 HTML 文件。 |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | 指示当文件只有一个工作表时是否导出单个标签页。 |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | 指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。 |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | 指示在保存文件之前是否合并条件格式和验证的区域。 |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | HTML 页面标题。 |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | 解析单元格中的 HTML 标签，例如 |

,作为单元格值，或作为 html 标签，默认是 true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | 指示 html 或 mht 文件是否为呈现首选项。默认值为 false。如果您想获得更美观的呈现，请将该值设置为 true。 |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | 指示是否刷新图表缓存数据 |
| [setSortNames(boolean value)](#setSortNames-boolean-) | 指示在保存文件之前是否对已定义名称进行排序。 |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | 指示在保存文件之前是否验证合并的单元格。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


创建用于保存 html 文件的选项。

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


创建用于保存 htm 文件的选项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat)。保存文件的格式。 |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


附加文件将保存到的目录。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


指定附加文件（如 html 文件中的图像）的 Url 前缀。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


缓存文件夹用于存储一些大数据。

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


在保存文件后使工作簿为空。

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


如果未设置，则使用 Encoding.UTF8 作为默认编码类型。

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


指示是否将整个工作簿导出为 HTML 文件。

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


获取当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存文件为 html 时，仅会导出指定的区域。

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


指示是否导出网格线。默认值为 false。

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


指示在将文件保存为 html 时是否导出标题。默认值为 false。如果您想将 html 文件导入到 excel，请保持默认值。

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


指示是否导出隐藏工作表的内容。默认值为 true。

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


指示是否仅导出打印区域到 HTML 文件。默认值为 false。

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


HTML 页面标题。仅用于保存为 html 流。

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


解析单元格中的 HTML 标签，例如

,作为单元格值，或作为 html 标签，默认是 true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


指示 html 或 mht 文件是否为呈现首选项。默认值为 false。如果您想获得更美观的呈现，请将该值设置为 true。

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


指示是否刷新图表缓存数据

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取保存的文件格式。

参见 [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


指示在保存文件之前是否对已定义名称进行排序。

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


指示在将文件保存为 HTML 时是否导出注释，默认值为 false。

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。默认值为 false。

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




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


附加文件将保存到的目录。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


指定附加文件（如 html 文件中的图像）的 Url 前缀。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


缓存文件夹用于存储一些大数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


在保存文件后使工作簿为空。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


如果为 true 且目录不存在，目录将在保存文件之前自动创建。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


指定导出 html 时的默认字体名称，当样式的字体不存在时将使用默认字体；如果此属性为 null，Aspose.Cells 将使用与原始字体同一系列的通用字体，默认值为 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


如果未设置，则使用 Encoding.UTF8 作为默认编码类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


指示是否将整个工作簿导出为 HTML 文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


设置当前活动工作表的导出 CellArea。如果设置此属性，当前活动工作表的打印区域将被省略。保存文件为 html 时，仅会导出指定的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


指示在将文件保存为 HTML 时是否导出注释，默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


指示是否导出网格线。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


指示在将文件保存为 html 时是否导出标题。默认值为 false。如果您想将 html 文件导入到 excel，请保持默认值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


指示是否导出隐藏工作表的内容。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


指定图像是否以 Base64 格式保存到 HTML、MHTML 或 EPUB。

**Remarks**

当此属性设置为 true 时，图像数据直接导出到 img 元素上，不会创建单独的文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


指示是否仅导出打印区域到 HTML 文件。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


指示当文件仅包含一个工作表时是否导出单个标签页。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


指示在 sheet00x.htm、filelist.xml 和 tabstrip.htm 中是否使用完整路径链接。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


指示在保存文件之前是否合并条件格式和验证的区域。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


HTML 页面标题。仅用于保存为 html 流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


解析单元格中的 HTML 标签，例如

,作为单元格值，或作为 html 标签，默认是 true

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


指示 html 或 mht 文件是否为呈现首选项。默认值为 false。如果您想获得更美观的呈现，请将该值设置为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


指示是否刷新图表缓存数据

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


指示在保存文件之前是否对已定义名称进行排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


指示在保存文件之前是否验证合并的单元格。

**Remarks**

默认值为 false。

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

