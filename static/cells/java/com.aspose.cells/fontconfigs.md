##FontConfigs
Specifies font settings
**Inheritance:**
java.lang.Object
```
public class FontConfigs
```
Specifies font settings
## Constructors
| Constructor | Description |
| --- | --- |
| [FontConfigs()](#FontConfigs--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefaultFontName()](#getDefaultFontName--) | Gets the default font name. |
| [getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)](#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-) | Get data infomation of font file data. |
| [getFontSources()](#getFontSources--) | Gets a copy of the array that contains the list of sources |
| [getFontSubstitutes(String originalFontName)](#getFontSubstitutes-java.lang.String-) | Returns array containing font substitute names to be used if original font is not presented. |
| [hashCode()](#hashCode--) |  |
| [isFontAvailable(String fontName)](#isFontAvailable-java.lang.String-) | Indicate whether the font is available. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Sets the default font name. |
| [setFontExclusiveSources(FontSourceBase[] exclusiveSources)](#setFontExclusiveSources-com.aspose.cells.FontSourceBase---) | Sets the fonts exclusive sources. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Sets the fonts folder |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Sets the fonts folders |
| [setFontSources(FontSourceBase[] sources)](#setFontSources-com.aspose.cells.FontSourceBase---) | Sets the fonts sources. |
| [setFontSubstitutes(String originalFontName, String[] substituteFontNames)](#setFontSubstitutes-java.lang.String-java.lang.String---) | Font substitute names for given original font name. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FontConfigs() {#FontConfigs--}
```
public FontConfigs()
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
### getDefaultFontName() {#getDefaultFontName--}
```
public static String getDefaultFontName()
```
Gets the default font name.
**Returns:**
java.lang.String
### getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle) {#getFontFileDataInfo-java.lang.String-boolean-boolean-boolean-}
```
public static FontFileDataInfo getFontFileDataInfo(String fontName, boolean isBold, boolean isItalic, boolean isExactStyle)
```
Get data infomation of font file data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | font name |
| isBold | boolean | the font style is bold or not |
| isItalic | boolean | the font style is italic or not |
| isExactStyle | boolean | whether to match the given bold/italic style exactly |
**Returns:**
[FontFileDataInfo](../../com.aspose.cells/fontfiledatainfo) - Data infomation of font file data.
### getFontSources() {#getFontSources--}
```
public static FontSourceBase[] getFontSources()
```
Gets a copy of the array that contains the list of sources
**Returns:**
com.aspose.cells.FontSourceBase[] -
### getFontSubstitutes(String originalFontName) {#getFontSubstitutes-java.lang.String-}
```
public static String[] getFontSubstitutes(String originalFontName)
```
Returns array containing font substitute names to be used if original font is not presented.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | originalFontName |
**Returns:**
java.lang.String[] - An array containing font substitute names to be used if original font is not presented.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isFontAvailable(String fontName) {#isFontAvailable-java.lang.String-}
```
public static boolean isFontAvailable(String fontName)
```
Indicate whether the font is available.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | font name |
**Returns:**
boolean - true if font is available, otherwise false.
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public static void setDefaultFontName(String value)
```
Sets the default font name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFontExclusiveSources(FontSourceBase[] exclusiveSources) {#setFontExclusiveSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontExclusiveSources(FontSourceBase[] exclusiveSources)
```
Sets the fonts exclusive sources. Only fonts in the sources will be used.
**Remarks**
System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") will be ignored if this is set.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| exclusiveSources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | An array of sources that contain TrueType fonts. |
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
### setFontSources(FontSourceBase[] sources) {#setFontSources-com.aspose.cells.FontSourceBase---}
```
public static void setFontSources(FontSourceBase[] sources)
```
Sets the fonts sources.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase\[\]](../../com.aspose.cells/fontsourcebase) | An array of sources that contain TrueType fonts. |
### setFontSubstitutes(String originalFontName, String[] substituteFontNames) {#setFontSubstitutes-java.lang.String-java.lang.String---}
```
public static void setFontSubstitutes(String originalFontName, String[] substituteFontNames)
```
Font substitute names for given original font name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | java.lang.String | Original font name. |
| substituteFontNames | java.lang.String[] | List of font substitute names to be used if original font is not presented. |
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
