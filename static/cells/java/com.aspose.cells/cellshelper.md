##CellsHelper
Provides helper functions.
**Inheritance:**
java.lang.Object
```
public class CellsHelper
```
Provides helper functions.
## Methods
| Method | Description |
| --- | --- |
| [addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)](#addAddInFunction-java.lang.String-int-int-int---int-) | Add addin function. |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | Gets cell name according to its row and column indexes. |
| [cellNameToIndex(String cellName)](#cellNameToIndex-java.lang.String-) | Gets the cell row and column indexes according to its name. |
| [columnIndexToName(int column)](#columnIndexToName-int-) | Gets column name according to column index. |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | Gets column index according to column name. |
| [convertA1FormulaToR1C1(String formula, int row, int column)](#convertA1FormulaToR1C1-java.lang.String-int-int-) | Converts A1 formula of the cell to the r1c1 formula. |
| [convertR1C1FormulaToA1(String r1c1Formula, int row, int column)](#convertR1C1FormulaToA1-java.lang.String-int-int-) | Converts the r1c1 formula of the cell to A1 formula. |
| [createSafeSheetName(String nameProposal)](#createSafeSheetName-java.lang.String-) | Checks given sheet name and create a valid one when needed. |
| [createSafeSheetName(String nameProposal, char replaceChar)](#createSafeSheetName-java.lang.String-char-) | Checks given sheet name and create a valid one when needed. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAltStartPath()](#getAltStartPath--) | Gets the alternate startup path, which is referred to by some external formula references. |
| [getCacheFolder()](#getCacheFolder--) | Gets the folder for temporary files that may be used as data cache. |
| [getClass()](#getClass--) |  |
| [getCustomImplementationFactory()](#getCustomImplementationFactory--) | Gets the factory for creating instances with special implementation. |
| [getDPI()](#getDPI--) | Gets the DPI of the machine. |
| [getDateTimeFromDouble(double doubleValue, boolean date1904)](#getDateTimeFromDouble-double-boolean-) | Convert the double value to the date time value. |
| [getDoubleFromDateTime(DateTime dateTime, boolean date1904)](#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-) | Convert the date time to double value. |
| [getLibraryPath()](#getLibraryPath--) | Gets the library path which is referred to by some external formula references. |
| [getSignificantDigits()](#getSignificantDigits--) | Gets the number of significant digits. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Gets the default type of significant digits for outputing numeric values. |
| [getStartupPath()](#getStartupPath--) | Gets the startup path, which is referred to by some external formula references. |
| [getTextWidth(String text, Font font, double scaling)](#getTextWidth-java.lang.String-com.aspose.cells.Font-double-) | Get width of text in unit of points. |
| [getUsedColors(Workbook workbook)](#getUsedColors-com.aspose.cells.Workbook-) | Gets all used colors in the workbook. |
| [getVersion()](#getVersion--) | Get the release version. |
| [hashCode()](#hashCode--) |  |
| [isCloudPlatform()](#isCloudPlatform--) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [mergeFiles(String[] files, String cachedFile, String destFile)](#mergeFiles-java.lang.String---java.lang.String-java.lang.String-) | Merges some large xls files to a xls file. |
| [needQuoteInFormula(String sheetName)](#needQuoteInFormula-java.lang.String-) | Indicates whether the name of the sheet should be enclosed in single quotes |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [rowIndexToName(int row)](#rowIndexToName-int-) | Gets row name according to row index. |
| [rowNameToIndex(String rowName)](#rowNameToIndex-java.lang.String-) | Gets row index according to row name. |
| [setAltStartPath(String value)](#setAltStartPath-java.lang.String-) | Sets the alternate startup path, which is referred to by some external formula references. |
| [setCacheFolder(String cache)](#setCacheFolder-java.lang.String-) | Sets the folder for temporary files that may be used as data cache. |
| [setCloudPlatform(boolean value)](#setCloudPlatform-boolean-) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |
| [setCustomImplementationFactory(CustomImplementationFactory value)](#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-) | Sets the factory for creating instances with special implementation. |
| [setDPI(double value)](#setDPI-double-) | Gets the DPI of the machine. |
| [setLibraryPath(String value)](#setLibraryPath-java.lang.String-) | Sets the library path which is referred to by some external formula references. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Sets the number of significant digits. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Sets the default type of significant digits for outputing numeric values. |
| [setStartupPath(String value)](#setStartupPath-java.lang.String-) | Sets the startup path, which is referred to by some external formula references. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType) {#addAddInFunction-java.lang.String-int-int-int---int-}
```
public static void addAddInFunction(String function, int minCountOfParameters, int maxCountOfParameters, int[] paramersType, int functionValueType)
```
Add addin function.
**Remarks**
NOTE: This member is now obsolete. Instead, please use WorksheetCollection.RegisterAddInFunction() methods. This method will be removed 12 months later since January 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| function | java.lang.String | The function name. |
| minCountOfParameters | int | Minimum number of parameters this function requires |
| maxCountOfParameters | int | Maximum number of parameters this function allows. |
| paramersType | int[] | [ParameterType](../../com.aspose.cells/parametertype). The excepted parameters type of the function |
| functionValueType | int | [ParameterType](../../com.aspose.cells/parametertype). The function value type. |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```
Gets cell name according to its row and column indexes.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
| column | int | Column index. |
**Returns:**
java.lang.String - Name of cell.
### cellNameToIndex(String cellName) {#cellNameToIndex-java.lang.String-}
```
public static int[] cellNameToIndex(String cellName)
```
Gets the cell row and column indexes according to its name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | java.lang.String | Name of cell |
**Returns:**
int[] - [0] is the row index and [1] is the column index.
### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```
Gets column name according to column index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | int | Column index. |
**Returns:**
java.lang.String - Name of column.
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```
Gets column index according to column name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnName | java.lang.String | Column name. |
**Returns:**
int - Column index.
### convertA1FormulaToR1C1(String formula, int row, int column) {#convertA1FormulaToR1C1-java.lang.String-int-int-}
```
public static String convertA1FormulaToR1C1(String formula, int row, int column)
```
Converts A1 formula of the cell to the r1c1 formula.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The A1 formula. |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |
**Returns:**
java.lang.String - The R1C1 formula.
### convertR1C1FormulaToA1(String r1c1Formula, int row, int column) {#convertR1C1FormulaToA1-java.lang.String-int-int-}
```
public static String convertR1C1FormulaToA1(String r1c1Formula, int row, int column)
```
Converts the r1c1 formula of the cell to A1 formula.
**Remarks**
NOTE: This member is now obsolete. Instead, please use Worksheet.ConvertFormulaReferenceStyle() method. This property will be removed 12 months later since August 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| r1c1Formula | java.lang.String | The r1c1 formula. |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |
**Returns:**
java.lang.String - The A1 formula.
### createSafeSheetName(String nameProposal) {#createSafeSheetName-java.lang.String-}
```
public static String createSafeSheetName(String nameProposal)
```
Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with ' ', then return the rebuilt string value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | java.lang.String | sheet name to be used |
**Returns:**
java.lang.String -
### createSafeSheetName(String nameProposal, char replaceChar) {#createSafeSheetName-java.lang.String-char-}
```
public static String createSafeSheetName(String nameProposal, char replaceChar)
```
Checks given sheet name and create a valid one when needed. If given sheet name conforms to the rules of excel sheet name, then return it. Otherwise string will be truncated if length exceeds the limit and invalid characters will be replaced with given character, then return the rebuilt string value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| nameProposal | java.lang.String | sheet name to be used |
| replaceChar | char | character which will be used to replace invalid characters in given sheet name |
**Returns:**
java.lang.String -
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
### getAltStartPath() {#getAltStartPath--}
```
public static String getAltStartPath()
```
Gets the alternate startup path, which is referred to by some external formula references.
**Returns:**
java.lang.String
### getCacheFolder() {#getCacheFolder--}
```
public static String getCacheFolder()
```
Gets the folder for temporary files that may be used as data cache.
**Remarks**
Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.
**Returns:**
java.lang.String - Folder for cache files that has been specified. If it has not been specified, null will be returned and system's temporary path will be used when needed.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCustomImplementationFactory() {#getCustomImplementationFactory--}
```
public static CustomImplementationFactory getCustomImplementationFactory()
```
Gets the factory for creating instances with special implementation.
**Returns:**
[CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory)
### getDPI() {#getDPI--}
```
public static double getDPI()
```
Gets the DPI of the machine.
**Remarks**
**Returns:**
double
### getDateTimeFromDouble(double doubleValue, boolean date1904) {#getDateTimeFromDouble-double-boolean-}
```
public static DateTime getDateTimeFromDouble(double doubleValue, boolean date1904)
```
Convert the double value to the date time value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | double | The double value. |
| date1904 | boolean | Date 1904 system. |
**Returns:**
[DateTime](../../com.aspose.cells/datetime) -
### getDoubleFromDateTime(DateTime dateTime, boolean date1904) {#getDoubleFromDateTime-com.aspose.cells.DateTime-boolean-}
```
public static double getDoubleFromDateTime(DateTime dateTime, boolean date1904)
```
Convert the date time to double value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | The date time. |
| date1904 | boolean | Date 1904 system. |
**Returns:**
double -
### getLibraryPath() {#getLibraryPath--}
```
public static String getLibraryPath()
```
Gets the library path which is referred to by some external formula references.
**Returns:**
java.lang.String
### getSignificantDigits() {#getSignificantDigits--}
```
public static int getSignificantDigits()
```
Gets the number of significant digits. The default value is 17.
**Remarks**
Only could be 15 or 17 now. NOTE: This member is now obsolete. Instead, please use [WorkbookSettings.getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). This property will be removed 12 months later since June 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public static int getSignificantDigitsType()
```
Gets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).
See [WorkbookSettings.getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--).
**Returns:**
int
### getStartupPath() {#getStartupPath--}
```
public static String getStartupPath()
```
Gets the startup path, which is referred to by some external formula references.
**Returns:**
java.lang.String
### getTextWidth(String text, Font font, double scaling) {#getTextWidth-java.lang.String-com.aspose.cells.Font-double-}
```
public static double getTextWidth(String text, Font font, double scaling)
```
Get width of text in unit of points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text. |
| font | [Font](../../com.aspose.cells/font) | The font of the text. |
| scaling | double | The scaling of text. |
**Returns:**
double -
### getUsedColors(Workbook workbook) {#getUsedColors-com.aspose.cells.Workbook-}
```
public static Color[] getUsedColors(Workbook workbook)
```
Gets all used colors in the workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | The workbook object. |
**Returns:**
com.aspose.cells.Color[] - The used colors.
### getVersion() {#getVersion--}
```
public static String getVersion()
```
Get the release version.
**Returns:**
java.lang.String - The release version.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isCloudPlatform() {#isCloudPlatform--}
```
public static boolean isCloudPlatform()
```
Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,
**Returns:**
boolean
### mergeFiles(String[] files, String cachedFile, String destFile) {#mergeFiles-java.lang.String---java.lang.String-java.lang.String-}
```
public static void mergeFiles(String[] files, String cachedFile, String destFile)
```
Merges some large xls files to a xls file.
**Remarks**
This method only supports merging data, style and formulas to the new file. The cached file is used to store some temporary data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| files | java.lang.String[] | The files. |
| cachedFile | java.lang.String | The cached file. |
| destFile | java.lang.String | The dest file. |
### needQuoteInFormula(String sheetName) {#needQuoteInFormula-java.lang.String-}
```
public static boolean needQuoteInFormula(String sheetName)
```
Indicates whether the name of the sheet should be enclosed in single quotes
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | The name of the sheet |
**Returns:**
boolean -
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### rowIndexToName(int row) {#rowIndexToName-int-}
```
public static String rowIndexToName(int row)
```
Gets row name according to row index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | Row index. |
**Returns:**
java.lang.String - Name of row.
### rowNameToIndex(String rowName) {#rowNameToIndex-java.lang.String-}
```
public static int rowNameToIndex(String rowName)
```
Gets row index according to row name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowName | java.lang.String | Row name. |
**Returns:**
int - Row index.
### setAltStartPath(String value) {#setAltStartPath-java.lang.String-}
```
public static void setAltStartPath(String value)
```
Sets the alternate startup path, which is referred to by some external formula references.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCacheFolder(String cache) {#setCacheFolder-java.lang.String-}
```
public static void setCacheFolder(String cache)
```
Sets the folder for temporary files that may be used as data cache.
**Remarks**
Cache files are used generally for some features for memory performance consideration, such as saving large data set to xls file, or using memory mode with file cache for cells model.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cache | java.lang.String | Folder for for temporary files that may be used as data cache. |
### setCloudPlatform(boolean value) {#setCloudPlatform-boolean-}
```
public static void setCloudPlatform(boolean value)
```
Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc,
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCustomImplementationFactory(CustomImplementationFactory value) {#setCustomImplementationFactory-com.aspose.cells.CustomImplementationFactory-}
```
public static void setCustomImplementationFactory(CustomImplementationFactory value)
```
Sets the factory for creating instances with special implementation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomImplementationFactory](../../com.aspose.cells/customimplementationfactory) |  |
### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```
Gets the DPI of the machine.
**Remarks**
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setLibraryPath(String value) {#setLibraryPath-java.lang.String-}
```
public static void setLibraryPath(String value)
```
Sets the library path which is referred to by some external formula references.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public static void setSignificantDigits(int value)
```
Sets the number of significant digits. The default value is 17.
**Remarks**
Only could be 15 or 17 now. NOTE: This member is now obsolete. Instead, please use [WorkbookSettings.getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). This property will be removed 12 months later since June 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public static void setSignificantDigitsType(int value)
```
Sets the default type of significant digits for outputing numeric values. Default value is [SignificantDigitsType.G\_17](../../com.aspose.cells/significantdigitstype\#G-17).
See [WorkbookSettings.getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStartupPath(String value) {#setStartupPath-java.lang.String-}
```
public static void setStartupPath(String value)
```
Sets the startup path, which is referred to by some external formula references.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
