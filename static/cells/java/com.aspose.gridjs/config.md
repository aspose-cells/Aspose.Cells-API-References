##Config
Represents all the static settings for GridJs
**Inheritance:**
java.lang.Object
```
public class Config
```
Represents all the static settings for GridJs
## Constructors
| Constructor | Description |
| --- | --- |
| [Config()](#Config--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoOptimizeForLargeCells()](#getAutoOptimizeForLargeCells--) | Gets whether to automatically optimize the load performance for worksheet with large cells. |
| [getBaseRouteName()](#getBaseRouteName--) | Gets the base route name for GridJs controller URL. the default is "/GridJs2". |
| [getClass()](#getClass--) |  |
| [getEmptySheetMaxCol()](#getEmptySheetMaxCol--) | Gets default max column for an empty worksheet. |
| [getEmptySheetMaxRow()](#getEmptySheetMaxRow--) | Gets default max row for an empty worksheet. |
| [getFileCacheDirectory()](#getFileCacheDirectory--) | Gets the cache directory for storing spreadsheet file. |
| [getIgnoreEmptyContent()](#getIgnoreEmptyContent--) | Gets whether to show the max range which includes data ,style, merged cells and shapes. |
| [getIslimitShapeOrImage()](#getIslimitShapeOrImage--) | Gets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true. |
| [getLazyLoading()](#getLazyLoading--) | Gets whether to load active worksheet only,the default is false. |
| [getMaxPdfSaveSeconds()](#getMaxPdfSaveSeconds--) | Gets the max timed out seconds when save to PDF. |
| [getMaxShapeOrImageCount()](#getMaxShapeOrImageCount--) | Gets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. |
| [getMaxShapeOrImageWidthOrHeight()](#getMaxShapeOrImageWidthOrHeight--) | Gets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. |
| [getMaxTotalShapeOrImageCount()](#getMaxTotalShapeOrImageCount--) | Gets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. |
| [getMessageTopic()](#getMessageTopic--) | Gets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only. |
| [getPictureCacheDirectory()](#getPictureCacheDirectory--) | Gets the cache directory for pictures. |
| [getSameImageDetecting()](#getSameImageDetecting--) | Gets whether to check if images have same source,the default is true the default value is true. |
| [getSaveHtmlAsZip()](#getSaveHtmlAsZip--) | Gets whether to save html file as zip archive,the default is false. |
| [getShowChartSheet()](#getShowChartSheet--) | Gets whether to show chart worksheet. |
| [getSkipInvisibleShapes()](#getSkipInvisibleShapes--) | Gets whether to skip shapes that are invisble to UI ,the default value is true. |
| [getUsePrintArea()](#getUsePrintArea--) | Gets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. |
| [hashCode()](#hashCode--) |  |
| [isCollaborative()](#isCollaborative--) | Gets whether to support collabrative editing,the default is false. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoOptimizeForLargeCells(boolean value)](#setAutoOptimizeForLargeCells-boolean-) | Sets whether to automatically optimize the load performance for worksheet with large cells. |
| [setBaseRouteName(String value)](#setBaseRouteName-java.lang.String-) | Sets the base route name for GridJs controller URL. the default is "/GridJs2". |
| [setCollaborative(boolean value)](#setCollaborative-boolean-) | Sets whether to support collabrative editing,the default is false. |
| [setEmptySheetMaxCol(int value)](#setEmptySheetMaxCol-int-) | Sets default max column for an empty worksheet. |
| [setEmptySheetMaxRow(int value)](#setEmptySheetMaxRow-int-) | Sets default max row for an empty worksheet. |
| [setFileCacheDirectory(String value)](#setFileCacheDirectory-java.lang.String-) | Sets the cache directory for storing spreadsheet file. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Sets the fonts folder |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Sets the fonts folders |
| [setIgnoreEmptyContent(boolean value)](#setIgnoreEmptyContent-boolean-) | Sets whether to show the max range which includes data ,style, merged cells and shapes. |
| [setIslimitShapeOrImage(boolean value)](#setIslimitShapeOrImage-boolean-) | Sets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true. |
| [setLazyLoading(boolean value)](#setLazyLoading-boolean-) | Sets whether to load active worksheet only,the default is false. |
| [setMaxPdfSaveSeconds(int value)](#setMaxPdfSaveSeconds-int-) | Sets the max timed out seconds when save to PDF. |
| [setMaxShapeOrImageCount(int value)](#setMaxShapeOrImageCount-int-) | Sets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. |
| [setMaxShapeOrImageWidthOrHeight(int value)](#setMaxShapeOrImageWidthOrHeight-int-) | Sets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. |
| [setMaxTotalShapeOrImageCount(int value)](#setMaxTotalShapeOrImageCount-int-) | Sets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. |
| [setMessageTopic(String value)](#setMessageTopic-java.lang.String-) | Sets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only. |
| [setPictureCacheDirectory(String value)](#setPictureCacheDirectory-java.lang.String-) | Sets the cache directory for pictures. |
| [setSameImageDetecting(boolean value)](#setSameImageDetecting-boolean-) | Sets whether to check if images have same source,the default is true the default value is true. |
| [setSaveHtmlAsZip(boolean value)](#setSaveHtmlAsZip-boolean-) | Sets whether to save html file as zip archive,the default is false. |
| [setShowChartSheet(boolean value)](#setShowChartSheet-boolean-) | Sets whether to show chart worksheet. |
| [setSkipInvisibleShapes(boolean value)](#setSkipInvisibleShapes-boolean-) | Sets whether to skip shapes that are invisble to UI ,the default value is true. |
| [setUsePrintArea(boolean value)](#setUsePrintArea-boolean-) | Sets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Config() {#Config--}
```
public Config()
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
### getAutoOptimizeForLargeCells() {#getAutoOptimizeForLargeCells--}
```
public static boolean getAutoOptimizeForLargeCells()
```
Gets whether to automatically optimize the load performance for worksheet with large cells. it will ignore some style /borders to reduce the load time. the default value is true.
**Returns:**
boolean
### getBaseRouteName() {#getBaseRouteName--}
```
public static String getBaseRouteName()
```
Gets the base route name for GridJs controller URL. the default is "/GridJs2".
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
Gets default max column for an empty worksheet. the default value is 15.
**Returns:**
int
### getEmptySheetMaxRow() {#getEmptySheetMaxRow--}
```
public static int getEmptySheetMaxRow()
```
Gets default max row for an empty worksheet. the default value is 12.
**Returns:**
int
### getFileCacheDirectory() {#getFileCacheDirectory--}
```
public static String getFileCacheDirectory()
```
Gets the cache directory for storing spreadsheet file. We need to set it to a specific path before we use GridJs.
**Returns:**
java.lang.String
### getIgnoreEmptyContent() {#getIgnoreEmptyContent--}
```
public static boolean getIgnoreEmptyContent()
```
Gets whether to show the max range which includes data ,style, merged cells and shapes. if the last row or column contains cells with no value and formula but has custom style then we will not show this row/column when this vlaue is true\\u9286?\* the default value is true .
**Returns:**
boolean
### getIslimitShapeOrImage() {#getIslimitShapeOrImage--}
```
public static boolean getIslimitShapeOrImage()
```
Gets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true.
**Returns:**
boolean
### getLazyLoading() {#getLazyLoading--}
```
public static boolean getLazyLoading()
```
Gets whether to load active worksheet only,the default is false.
**Returns:**
boolean
### getMaxPdfSaveSeconds() {#getMaxPdfSaveSeconds--}
```
public static int getMaxPdfSaveSeconds()
```
Gets the max timed out seconds when save to PDF. the default value is 10.
**Returns:**
int
### getMaxShapeOrImageCount() {#getMaxShapeOrImageCount--}
```
public static int getMaxShapeOrImageCount()
```
Gets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. the default value is 100.
**Returns:**
int
### getMaxShapeOrImageWidthOrHeight() {#getMaxShapeOrImageWidthOrHeight--}
```
public static int getMaxShapeOrImageWidthOrHeight()
```
Gets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. the default value is 10000.
**Returns:**
int
### getMaxTotalShapeOrImageCount() {#getMaxTotalShapeOrImageCount--}
```
public static int getMaxTotalShapeOrImageCount()
```
Gets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. the default value is 300.
**Returns:**
int
### getMessageTopic() {#getMessageTopic--}
```
public static String getMessageTopic()
```
Gets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only.
**Returns:**
java.lang.String
### getPictureCacheDirectory() {#getPictureCacheDirectory--}
```
public static String getPictureCacheDirectory()
```
Gets the cache directory for pictures.(this takes effect when GridJsWorkbook.CacheImp is null) the default path will be "\_piccache" inside the FileCacheDirectory.
**Returns:**
java.lang.String
### getSameImageDetecting() {#getSameImageDetecting--}
```
public static boolean getSameImageDetecting()
```
Gets whether to check if images have same source,the default is true the default value is true.
**Returns:**
boolean
### getSaveHtmlAsZip() {#getSaveHtmlAsZip--}
```
public static boolean getSaveHtmlAsZip()
```
Gets whether to save html file as zip archive,the default is false.
**Returns:**
boolean
### getShowChartSheet() {#getShowChartSheet--}
```
public static boolean getShowChartSheet()
```
Gets whether to show chart worksheet. the default value is false .
**Returns:**
boolean
### getSkipInvisibleShapes() {#getSkipInvisibleShapes--}
```
public static boolean getSkipInvisibleShapes()
```
Gets whether to skip shapes that are invisble to UI ,the default value is true.
**Returns:**
boolean
### getUsePrintArea() {#getUsePrintArea--}
```
public static boolean getUsePrintArea()
```
Gets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. the default value is false .
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
Gets whether to support collabrative editing,the default is false.
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
### setAutoOptimizeForLargeCells(boolean value) {#setAutoOptimizeForLargeCells-boolean-}
```
public static void setAutoOptimizeForLargeCells(boolean value)
```
Sets whether to automatically optimize the load performance for worksheet with large cells. it will ignore some style /borders to reduce the load time. the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBaseRouteName(String value) {#setBaseRouteName-java.lang.String-}
```
public static void setBaseRouteName(String value)
```
Sets the base route name for GridJs controller URL. the default is "/GridJs2".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCollaborative(boolean value) {#setCollaborative-boolean-}
```
public static void setCollaborative(boolean value)
```
Sets whether to support collabrative editing,the default is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmptySheetMaxCol(int value) {#setEmptySheetMaxCol-int-}
```
public static void setEmptySheetMaxCol(int value)
```
Sets default max column for an empty worksheet. the default value is 15.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEmptySheetMaxRow(int value) {#setEmptySheetMaxRow-int-}
```
public static void setEmptySheetMaxRow(int value)
```
Sets default max row for an empty worksheet. the default value is 12.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFileCacheDirectory(String value) {#setFileCacheDirectory-java.lang.String-}
```
public static void setFileCacheDirectory(String value)
```
Sets the cache directory for storing spreadsheet file. We need to set it to a specific path before we use GridJs.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```
Sets the fonts folder
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | java.lang.String | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |
### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```
Sets the fonts folders
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | java.lang.String[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |
### setIgnoreEmptyContent(boolean value) {#setIgnoreEmptyContent-boolean-}
```
public static void setIgnoreEmptyContent(boolean value)
```
Sets whether to show the max range which includes data ,style, merged cells and shapes. if the last row or column contains cells with no value and formula but has custom style then we will not show this row/column when this vlaue is true\\u9286?\* the default value is true .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setIslimitShapeOrImage(boolean value) {#setIslimitShapeOrImage-boolean-}
```
public static void setIslimitShapeOrImage(boolean value)
```
Sets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLazyLoading(boolean value) {#setLazyLoading-boolean-}
```
public static void setLazyLoading(boolean value)
```
Sets whether to load active worksheet only,the default is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMaxPdfSaveSeconds(int value) {#setMaxPdfSaveSeconds-int-}
```
public static void setMaxPdfSaveSeconds(int value)
```
Sets the max timed out seconds when save to PDF. the default value is 10.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMaxShapeOrImageCount(int value) {#setMaxShapeOrImageCount-int-}
```
public static void setMaxShapeOrImageCount(int value)
```
Sets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. the default value is 100.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMaxShapeOrImageWidthOrHeight(int value) {#setMaxShapeOrImageWidthOrHeight-int-}
```
public static void setMaxShapeOrImageWidthOrHeight(int value)
```
Sets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. the default value is 10000.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMaxTotalShapeOrImageCount(int value) {#setMaxTotalShapeOrImageCount-int-}
```
public static void setMaxTotalShapeOrImageCount(int value)
```
Sets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. the default value is 300.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMessageTopic(String value) {#setMessageTopic-java.lang.String-}
```
public static void setMessageTopic(String value)
```
Sets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPictureCacheDirectory(String value) {#setPictureCacheDirectory-java.lang.String-}
```
public static void setPictureCacheDirectory(String value)
```
Sets the cache directory for pictures.(this takes effect when GridJsWorkbook.CacheImp is null) the default path will be "\_piccache" inside the FileCacheDirectory.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSameImageDetecting(boolean value) {#setSameImageDetecting-boolean-}
```
public static void setSameImageDetecting(boolean value)
```
Sets whether to check if images have same source,the default is true the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSaveHtmlAsZip(boolean value) {#setSaveHtmlAsZip-boolean-}
```
public static void setSaveHtmlAsZip(boolean value)
```
Sets whether to save html file as zip archive,the default is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowChartSheet(boolean value) {#setShowChartSheet-boolean-}
```
public static void setShowChartSheet(boolean value)
```
Sets whether to show chart worksheet. the default value is false .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSkipInvisibleShapes(boolean value) {#setSkipInvisibleShapes-boolean-}
```
public static void setSkipInvisibleShapes(boolean value)
```
Sets whether to skip shapes that are invisble to UI ,the default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setUsePrintArea(boolean value) {#setUsePrintArea-boolean-}
```
public static void setUsePrintArea(boolean value)
```
Sets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. the default value is false .
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
