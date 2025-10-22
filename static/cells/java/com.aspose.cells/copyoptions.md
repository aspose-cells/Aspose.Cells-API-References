##CopyOptions
Represents the copy options.
**Inheritance:**
java.lang.Object
```
public class CopyOptions
```
Represents the copy options.
## Constructors
| Constructor | Description |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions constructor. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indicates whether copying column width in unit of characters. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | If the formula is not valid for the dest destination, only copy values. |
| [getCopyNames()](#getCopyNames--) | Indicates whether copying the names. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indicates whether extend ranges when copying the range to adjacent range. |
| [getKeepMacros()](#getKeepMacros--) | Indicates whether keeping macros; |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | Indicates whether copying column width in unit of characters. |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | If the formula is not valid for the dest destination, only copy values. |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | Indicates whether copying the names. |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | Indicates whether extend ranges when copying the range to adjacent range. |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | Indicates whether keeping macros; |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```
CopyOptions constructor.
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
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```
Indicates whether copying column width in unit of characters.
**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```
If the formula is not valid for the dest destination, only copy values.
**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```
Indicates whether copying the names.
**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```
Indicates whether extend ranges when copying the range to adjacent range.
**Remarks**
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```
Indicates whether keeping macros;
**Remarks**
Only for copying workbook.
**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```
When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.
**Remarks**
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.
**Remarks**
The default value is true.
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
### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```
Indicates whether copying column width in unit of characters.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```
If the formula is not valid for the dest destination, only copy values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```
Indicates whether copying the names.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```
Indicates whether extend ranges when copying the range to adjacent range.
**Remarks**
If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```
Indicates whether keeping macros;
**Remarks**
Only for copying workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```
When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.
**Remarks**
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.
**Remarks**
The default value is true.
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
