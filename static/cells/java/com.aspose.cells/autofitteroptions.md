##AutoFitterOptions
Represents all auto fitter options.
**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```
Represents all auto fitter options.
## Constructors
| Constructor | Description |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Indicates whether auto fit row height when the cells is merged in a row. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | Gets the type of auto fitting row height of merged cells. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | Gets the type of auto fitting wrapped text. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Gets default edit language. |
| [getForRendering()](#getForRendering--) | Indicates whether fit for rendering purpose. |
| [getFormatStrategy()](#getFormatStrategy--) | Gets the formatted strategy. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignores the hidden rows/columns. |
| [getMaxRowHeight()](#getMaxRowHeight--) | Gets the max row height(in unit of Point) when autofitting rows. |
| [getOnlyAuto()](#getOnlyAuto--) | Indicates whether only fit the rows which height are not customed. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | Indicates whether auto fit row height when the cells is merged in a row. |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | Sets the type of auto fitting row height of merged cells. |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | Sets the type of auto fitting wrapped text. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Sets default edit language. |
| [setForRendering(boolean value)](#setForRendering-boolean-) | Indicates whether fit for rendering purpose. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Sets the formatted strategy. |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | Ignores the hidden rows/columns. |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | Sets the max row height(in unit of Point) when autofitting rows. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Indicates whether only fit the rows which height are not customed. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```
Indicates whether auto fit row height when the cells is merged in a row. The default value is false.
**Remarks**
NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```
Gets the type of auto fitting row height of merged cells.
See [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).
**Remarks**
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```
Gets the type of auto fitting wrapped text.
See [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```
Gets default edit language.
See [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).
**Returns:**
int
### getForRendering() {#getForRendering--}
```
public boolean getForRendering()
```
Indicates whether fit for rendering purpose.
**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```
Gets the formatted strategy.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
**Remarks**
The default value is CellStyle for performance.
**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```
Ignores the hidden rows/columns.
**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```
Gets the max row height(in unit of Point) when autofitting rows.
**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```
Indicates whether only fit the rows which height are not customed.
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
### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```
Indicates whether auto fit row height when the cells is merged in a row. The default value is false.
**Remarks**
NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```
Sets the type of auto fitting row height of merged cells.
See [AutoFitMergedCellsType](../../com.aspose.cells/autofitmergedcellstype).
**Remarks**
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```
Sets the type of auto fitting wrapped text.
See [AutoFitWrappedTextType](../../com.aspose.cells/autofitwrappedtexttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```
Sets default edit language.
See [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setForRendering(boolean value) {#setForRendering-boolean-}
```
public void setForRendering(boolean value)
```
Indicates whether fit for rendering purpose.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```
Sets the formatted strategy.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
**Remarks**
The default value is CellStyle for performance.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```
Ignores the hidden rows/columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```
Sets the max row height(in unit of Point) when autofitting rows.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```
Indicates whether only fit the rows which height are not customed.
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
