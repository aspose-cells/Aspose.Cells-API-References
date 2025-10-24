##PivotFilter
Represents a PivotFilter in PivotFilter Collection.
**Inheritance:**
java.lang.Object
```
public class PivotFilter
```
Represents a PivotFilter in PivotFilter Collection.
**Example**
```
Workbook book = new Workbook();
Worksheet sheet = book.getWorksheets().get(0);
Cells cells = sheet.getCells();
cells.get(0, 0).setValue("fruit");
cells.get(1, 0).setValue("grape");
cells.get(2, 0).setValue("blueberry");
cells.get(3, 0).setValue("kiwi");
cells.get(4, 0).setValue("cherry");
cells.get(5, 0).setValue("grape");
cells.get(6, 0).setValue("blueberry");
cells.get(7, 0).setValue("kiwi");
cells.get(8, 0).setValue("cherry");
cells.get(0, 1).setValue("year");
cells.get(1, 1).setValue(2020);
cells.get(2, 1).setValue(2020);
cells.get(3, 1).setValue(2020);
cells.get(4, 1).setValue(2020);
cells.get(5, 1).setValue(2021);
cells.get(6, 1).setValue(2021);
cells.get(7, 1).setValue(2021);
cells.get(8, 1).setValue(2021);
cells.get(0, 2).setValue("amount");
cells.get(1, 2).setValue(50);
cells.get(2, 2).setValue(60);
cells.get(3, 2).setValue(70);
cells.get(4, 2).setValue(80);
cells.get(5, 2).setValue(90);
cells.get(6, 2).setValue(100);
cells.get(7, 2).setValue(110);
cells.get(8, 2).setValue(120);
PivotTableCollection pivots = sheet.getPivotTables();
int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots.get(pivotIndex);
pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
pivot.addFieldToArea(PivotFieldType.DATA, "amount");
pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
//Add top 10 filter
pivot.getBaseFields().get(0).filterTop10(0, PivotFilterType.COUNT,false,2);
pivot.refreshData();
pivot.calculateData();
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Gets the autofilter of the pivot filter. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | Gets values of the number filter. |
| [getEvaluationOrder()](#getEvaluationOrder--) | Gets the Evaluation Order of the pivot filter. |
| [getFieldIndex()](#getFieldIndex--) | Gets the index of source field which this pivot filter is applied to. |
| [getFilterCategory()](#getFilterCategory--) | Gets the category of this filter. |
| [getFilterType()](#getFilterType--) | Gets the autofilter type of the pivot filter. |
| [getLabels()](#getLabels--) | Gets labels of the caption filter. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | Specifies the index of the measure cube field. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Gets the measure field index of the pivot filter. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Gets the member property field index of the pivot filter. |
| [getName()](#getName--) | Gets the name of the pivot filter. |
| [getNumberValues()](#getNumberValues--) | Gets values of the number filter. |
| [getTop10Value()](#getTop10Value--) | Gets top 10 setting of the filter. |
| [getUseWholeDay()](#getUseWholeDay--) | Indicates whether uses whole days in its filtering criteria. |
| [getValue1()](#getValue1--) | Gets the string value1 of the label pivot filter. |
| [getValue2()](#getValue2--) | Gets the string value2 of the label pivot filter. |
| [getValueFieldIndex()](#getValueFieldIndex--) | Gets the index of value field in the value region. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | Gets the Evaluation Order of the pivot filter. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | Gets the measure field index of the pivot filter. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | Gets the member property field index of the pivot filter. |
| [setName(String value)](#setName-java.lang.String-) | Gets the name of the pivot filter. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | Indicates whether uses whole days in its filtering criteria. |
| [setValue1(String value)](#setValue1-java.lang.String-) | Gets the string value1 of the label pivot filter. |
| [setValue2(String value)](#setValue2-java.lang.String-) | Gets the string value2 of the label pivot filter. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | Gets the index of value field in the value region. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
public AutoFilter getAutoFilter()
```
Gets the autofilter of the pivot filter.
**Remarks**
NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDateTimeValues() {#getDateTimeValues--}
```
public DateTime[] getDateTimeValues()
```
Gets values of the number filter.
**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```
Gets the Evaluation Order of the pivot filter.
**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```
Gets the index of source field which this pivot filter is applied to.
**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```
Gets the category of this filter.
See [FilterCategory](../../com.aspose.cells/filtercategory).
**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```
Gets the autofilter type of the pivot filter.
See [PivotFilterType](../../com.aspose.cells/pivotfiltertype).
**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```
Gets labels of the caption filter.
**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```
Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.
**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```
Gets the measure field index of the pivot filter.
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```
Gets the member property field index of the pivot filter.
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Gets the name of the pivot filter.
**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```
Gets values of the number filter.
**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```
Gets top 10 setting of the filter.
**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```
Indicates whether uses whole days in its filtering criteria.
**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```
Gets the string value1 of the label pivot filter.
**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```
Gets the string value2 of the label pivot filter.
**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```
Gets the index of value field in the value region.
**Returns:**
int
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
### setEvaluationOrder(int value) {#setEvaluationOrder-int-}
```
public void setEvaluationOrder(int value)
```
Gets the Evaluation Order of the pivot filter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```
Gets the measure field index of the pivot filter.
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```
Gets the member property field index of the pivot filter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Gets the name of the pivot filter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```
Indicates whether uses whole days in its filtering criteria.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```
Gets the string value1 of the label pivot filter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```
Gets the string value2 of the label pivot filter.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```
Gets the index of value field in the value region.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
