---
title: GridHtmlSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options for saving html file.
type: docs
url: /java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

Represents the options for saving html file.
## Constructors

| Constructor | Description |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | Creates options for saving html file. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | Creates options for saving htm file. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | The directory that the attached files will be saved to. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Specify the Url prefix of attached files such as image in the html file. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getDefaultFontName()](#getDefaultFontName--) | Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null. |
| [getEncoding()](#getEncoding--) | If not set,use Encoding.UTF8 as default enconding type. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Indicates if exporting the whole workbook to html file. |
| [getExportArea()](#getExportArea--) | the exporting CellArea of current active Worksheet. |
| [getExportGridLines()](#getExportGridLines--) | Indicating whether exporting the gridlines.The default value is false. |
| [getExportHeadings()](#getExportHeadings--) | Indicates whether exporting headings when saving file to html.The default value is false. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Indicating if exporting the hidden worksheet content.The default value is true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Indicates if only exporting the print area to html file. |
| [getExportSingleTab()](#getExportSingleTab--) | Indicates whether exporting the single tab when the file only has one worksheet. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getPageTitle()](#getPageTitle--) | The title of the html page. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Parse html tag in cell,like

,as cell value,or as html tag,default is true |
| [getPresentationPreference()](#getPresentationPreference--) | Indicating if html or mht file is presentation preference.The default value is false.if you want to get more beautiful presentation,please set the value to true. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Indicates if exporting comments when saving file to html, the default value is false. |
| [isFullPathLink()](#isFullPathLink--) | Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getAttachedFilesDirectory--) |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | For the description of this property, please see [getAttachedFilesUrlPrefix()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getAttachedFilesUrlPrefix--) |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see [getCachedFileFolder()](../../com.aspose.gridweb/gridsaveoptions\#getCachedFileFolder--) |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see [getClearData()](../../com.aspose.gridweb/gridsaveoptions\#getClearData--) |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see [getCreateDirectory()](../../com.aspose.gridweb/gridsaveoptions\#getCreateDirectory--) |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | For the description of this property, please see [getDefaultFontName()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getDefaultFontName--) |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | For the description of this property, please see [getEncoding()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getEncoding--) |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | For the description of this property, please see [getExportActiveWorksheetOnly()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportActiveWorksheetOnly--) |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | For the description of this property, please see [getExportArea()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportArea--) |
| [setExportComments(boolean value)](#setExportComments-boolean-) | For the description of this property, please see [isExportComments()](../../com.aspose.gridweb/gridhtmlsaveoptions\#isExportComments--) |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | For the description of this property, please see [getExportGridLines()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportGridLines--) |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | For the description of this property, please see [getExportHeadings()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportHeadings--) |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | For the description of this property, please see [getExportHiddenWorksheet()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportHiddenWorksheet--) |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | For the description of this property, please see [getExportImagesAsBase64()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportImagesAsBase64--) |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | For the description of this property, please see [getExportPrintAreaOnly()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportPrintAreaOnly--) |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | For the description of this property, please see [getExportSingleTab()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportSingleTab--) |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | For the description of this property, please see [isFullPathLink()](../../com.aspose.gridweb/gridhtmlsaveoptions\#isFullPathLink--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see [getMergeAreas()](../../com.aspose.gridweb/gridsaveoptions\#getMergeAreas--) |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | For the description of this property, please see [getPageTitle()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getPageTitle--) |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | For the description of this property, please see [getParseHtmlTagInCell()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getParseHtmlTagInCell--) |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | For the description of this property, please see [getPresentationPreference()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getPresentationPreference--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see [getRefreshChartCache()](../../com.aspose.gridweb/gridsaveoptions\#getRefreshChartCache--) |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see [getSortNames()](../../com.aspose.gridweb/gridsaveoptions\#getSortNames--) |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.gridweb/gridsaveoptions\#getValidateMergedAreas--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


Creates options for saving html file.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


Creates options for saving htm file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The saving file format. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


The directory that the attached files will be saved to. Only for saving to html stream.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The cached file folder is used to store some large data.

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


Make the workbook empty after saving the file.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Specify the default font name for exporting html, the default font will be used when the font of style is not existing, If this property is null, Aspose.Cells will use universal font which have the same family with the original font, the default value is null.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


If not set,use Encoding.UTF8 as default enconding type.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Indicates if exporting the whole workbook to html file.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


the exporting CellArea of current active Worksheet. If you set this attribute, the print area of current active Worksheet will be omited. Only the specified area will be exported when saving the file to html.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Indicating whether exporting the gridlines.The default value is false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Indicates whether exporting headings when saving file to html.The default value is false. If you want to import the html file to excel, please keep the default value.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Indicating if exporting the hidden worksheet content.The default value is true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB. When this property is set to true image data is exported directly on the img elements and separate files are not created.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Indicates if only exporting the print area to html file. The default value is false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


The title of the html page. Only for saving to html stream.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Parse html tag in cell,like

,as cell value,or as html tag,default is true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Indicating if html or mht file is presentation preference.The default value is false.if you want to get more beautiful presentation,please set the value to true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indicates whether refreshing chart cache data

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the save file format.

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indicates whether sorting defined names before saving file.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file. The default value is false.

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


Indicates if exporting comments when saving file to html, the default value is false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Indicating whether using full path link in sheet00x.htm,filelist.xml and tabstrip.htm. The default value is false.

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


For the description of this property, please see [getAttachedFilesDirectory()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getAttachedFilesDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


For the description of this property, please see [getAttachedFilesUrlPrefix()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getAttachedFilesUrlPrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


For the description of this property, please see [getCachedFileFolder()](../../com.aspose.gridweb/gridsaveoptions\#getCachedFileFolder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


For the description of this property, please see [getClearData()](../../com.aspose.gridweb/gridsaveoptions\#getClearData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


For the description of this property, please see [getCreateDirectory()](../../com.aspose.gridweb/gridsaveoptions\#getCreateDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


For the description of this property, please see [getDefaultFontName()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getDefaultFontName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


For the description of this property, please see [getEncoding()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


For the description of this property, please see [getExportActiveWorksheetOnly()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportActiveWorksheetOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


For the description of this property, please see [getExportArea()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


For the description of this property, please see [isExportComments()](../../com.aspose.gridweb/gridhtmlsaveoptions\#isExportComments--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


For the description of this property, please see [getExportGridLines()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportGridLines--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


For the description of this property, please see [getExportHeadings()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportHeadings--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


For the description of this property, please see [getExportHiddenWorksheet()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportHiddenWorksheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


For the description of this property, please see [getExportImagesAsBase64()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportImagesAsBase64--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


For the description of this property, please see [getExportPrintAreaOnly()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportPrintAreaOnly--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


For the description of this property, please see [getExportSingleTab()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getExportSingleTab--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


For the description of this property, please see [isFullPathLink()](../../com.aspose.gridweb/gridhtmlsaveoptions\#isFullPathLink--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


For the description of this property, please see [getMergeAreas()](../../com.aspose.gridweb/gridsaveoptions\#getMergeAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


For the description of this property, please see [getPageTitle()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getPageTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


For the description of this property, please see [getParseHtmlTagInCell()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getParseHtmlTagInCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


For the description of this property, please see [getPresentationPreference()](../../com.aspose.gridweb/gridhtmlsaveoptions\#getPresentationPreference--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


For the description of this property, please see [getRefreshChartCache()](../../com.aspose.gridweb/gridsaveoptions\#getRefreshChartCache--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


For the description of this property, please see [getSortNames()](../../com.aspose.gridweb/gridsaveoptions\#getSortNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.gridweb/gridsaveoptions\#getValidateMergedAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

