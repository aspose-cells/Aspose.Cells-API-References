##GridTxtLoadOptions
Represents the options for loading text file.
**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
```
public class GridTxtLoadOptions extends GridLoadOptions
```
Represents the options for loading text file.
## Constructors
| Constructor | Description |
| --- | --- |
| [GridTxtLoadOptions()](#GridTxtLoadOptions--) | Creates the options for loading text file. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Indicates whether auto filtering the data when loading the files. |
| [getCheckDataValid()](#getCheckDataValid--) | Check whether data is valid in the template file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Gets a value that indicates whether the string in text file is converted to date data. |
| [getConvertNumericData()](#getConvertNumericData--) | Gets a value that indicates whether the string in text file is converted to numeric data. |
| [getEncoding()](#getEncoding--) | Gets the default encoding. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Whether extends data to next sheet when the rows or columns of data exceed limit. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignore the data which are not printed if directly printing the file |
| [getKeepPrecision()](#getKeepPrecision--) | Indicates whether not parsing a string value if the length is 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [getOnlyAuto()](#getOnlyAuto--) | Indicates whether only fit the rows which height are not customed. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Indicates whether parsing the formula when reading the file. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Indicates whether parsing pivot cached records when loading the file. |
| [getPassword()](#getPassword--) | Gets the password of the workbook. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [getSeparator()](#getSeparator--) | Gets character separator of text file. |
| [getSeparatorString()](#getSeparatorString--) | Gets a string value as separator. |
| [getTextQualifier()](#getTextQualifier--) | Specifies the text qualifier for cell values. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Whether consecutive delimiters should be treated as one. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. |
| [hasFormula()](#hasFormula--) | Indicates whether the text is formula if it starts with "=". |
| [hasTextQualifier()](#hasTextQualifier--) | Whether there is text qualifier for cell value. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | True means that the file contains several encoding. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Indicates whether auto filtering the data when loading the files. |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Check whether data is valid in the template file. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Sets a value that indicates whether the string in text file is converted to date data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Sets a value that indicates whether the string in text file is converted to numeric data. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Sets the default encoding. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Whether extends data to next sheet when the rows or columns of data exceed limit. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Indicates whether the text is formula if it starts with "=". |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Whether there is text qualifier for cell value. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignore the data which are not printed if directly printing the file |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Indicates whether not parsing a string value if the length is 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | True means that the file contains several encoding. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indicates whether only fit the rows which height are not customed. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Indicates whether parsing the formula when reading the file. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Indicates whether parsing pivot cached records when loading the file. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets the password of the workbook. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. |
| [setSeparator(char value)](#setSeparator-char-) | Sets character separator of text file. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Sets a string value as separator. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Specifies the text qualifier for cell values. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Whether consecutive delimiters should be treated as one. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Indicates whether the leading single quote sign should be taken as part of the value of one cell. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTxtLoadOptions() {#GridTxtLoadOptions--}
```
public GridTxtLoadOptions()
```
Creates the options for loading text file.
**Remarks**
The default load file type is CSV .
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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```
Indicates whether auto filtering the data when loading the files.
**Remarks**
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
**Returns:**
boolean
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```
Check whether data is valid in the template file.
**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```
Gets a value that indicates whether the string in text file is converted to date data.
**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```
Gets a value that indicates whether the string in text file is converted to numeric data.
**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```
Gets the default encoding. Only applies for csv file.
**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```
Whether extends data to next sheet when the rows or columns of data exceed limit. If this property is true, extra data will be extended to next sheet behind current one(if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeds limit will be ignored. Default is false;
**Returns:**
boolean
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```
Ignore the data which are not printed if directly printing the file
**Remarks**
Only for xlsx file.
**Returns:**
boolean
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```
Indicates whether not parsing a string value if the length is 15.
**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```
Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.
**Remarks**
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
**Returns:**
boolean
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```
Indicates whether only fit the rows which height are not customed.
**Returns:**
boolean
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```
Indicates whether parsing the formula when reading the file.
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```
Indicates whether parsing pivot cached records when loading the file. The default value is false.
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```
Gets the password of the workbook.
**Returns:**
java.lang.String
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
**Remarks**
After loading workbook from template file with this option, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) will be set to the same value with this property.
**Returns:**
boolean
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```
Gets character separator of text file.
**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```
Gets a string value as separator.
**Returns:**
java.lang.String
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```
Specifies the text qualifier for cell values. Default qualifier is '"'.
**Remarks**
When setting this property, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) will become true automatically.
**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```
Whether consecutive delimiters should be treated as one.
**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```
Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) will be set as true for the cell.
**Returns:**
boolean
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```
Indicates whether the text is formula if it starts with "=".
**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```
Whether there is text qualifier for cell value. Default is true.
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```
True means that the file contains several encoding.
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
### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```
Indicates whether auto filtering the data when loading the files.
**Remarks**
Sometimes although autofilter is set, the corresponding rows is not hidden in the file. Now only works for SpreadSheetML file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```
Check whether data is valid in the template file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```
Sets a value that indicates whether the string in text file is converted to date data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```
Sets a value that indicates whether the string in text file is converted to numeric data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```
Sets the default encoding. Only applies for csv file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |
### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```
Whether extends data to next sheet when the rows or columns of data exceed limit. If this property is true, extra data will be extended to next sheet behind current one(if current sheet is the last one, new sheet will be appended to current workbook). If this property is false, the data exceeds limit will be ignored. Default is false;
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```
Indicates whether the text is formula if it starts with "=".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```
Whether there is text qualifier for cell value. Default is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```
Ignore the data which are not printed if directly printing the file
**Remarks**
Only for xlsx file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```
Indicates whether not parsing a string value if the length is 15.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```
Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.
**Remarks**
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```
True means that the file contains several encoding.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```
Indicates whether only fit the rows which height are not customed.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```
Indicates whether parsing the formula when reading the file.
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm and Xlsm file because the formulas in the files are stored with a string formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```
Indicates whether parsing pivot cached records when loading the file. The default value is false.
**Remarks**
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```
Sets the password of the workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
**Remarks**
After loading workbook from template file with this option, [GridWorkbookSettings.getPreservePaddingSpaces()](../../com.aspose.gridweb/gridworkbooksettings\#getPreservePaddingSpaces--) will be set to the same value with this property.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```
Sets character separator of text file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |
### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```
Sets a string value as separator.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```
Specifies the text qualifier for cell values. Default qualifier is '"'.
**Remarks**
When setting this property, [hasTextQualifier()](../../com.aspose.gridweb/gridtxtloadoptions\#hasTextQualifier--) will become true automatically.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |
### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```
Whether consecutive delimiters should be treated as one.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```
Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [GridTableItemStyle.getQuotePrefix()](../../com.aspose.gridweb/gridtableitemstyle\#getQuotePrefix--) will be set as true for the cell.
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
