##PivotFilter
Represents a PivotFilter in PivotFilter Collection.
## PivotFilter class
Represents a PivotFilter in PivotFilter Collection.
```javascript
class PivotFilter;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [useWholeDay](#useWholeDay--)| boolean | Indicates whether uses whole days in its filtering criteria. |
| [autoFilter](#autoFilter--)| AutoFilter | Readonly. Gets the autofilter of the pivot filter. |
| [filterType](#filterType--)| PivotFilterType | Readonly. Gets the autofilter type of the pivot filter. |
| [fieldIndex](#fieldIndex--)| number | Readonly. Gets the index of source field which this pivot filter is applied to. |
| [filterCategory](#filterCategory--)| FilterCategory | Readonly. Gets the category of this filter. |
| [value1](#value1--)| string | Gets the string value1 of the label pivot filter. |
| [value2](#value2--)| string | Gets the string value2 of the label pivot filter. |
| [measureFldIndex](#measureFldIndex--)| number | Gets the measure field index of the pivot filter. |
| [valueFieldIndex](#valueFieldIndex--)| number | Gets the index of value field in the value region. |
| [measureCubeFieldIndex](#measureCubeFieldIndex--)| number | Readonly. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply. |
| [memberPropertyFieldIndex](#memberPropertyFieldIndex--)| number | Gets the member property field index of the pivot filter. |
| [name](#name--)| string | Gets the name of the pivot filter. |
| [evaluationOrder](#evaluationOrder--)| number | Gets the Evaluation Order of the pivot filter. |
## Methods
| Method | Description |
| --- | --- |
| [getUseWholeDay()](#getUseWholeDay--)| <b>@deprecated.</b> Please use the 'useWholeDay' property instead. Indicates whether uses whole days in its filtering criteria. |
| [setUseWholeDay(boolean)](#setUseWholeDay-boolean-)| <b>@deprecated.</b> Please use the 'useWholeDay' property instead. Indicates whether uses whole days in its filtering criteria. |
| [getAutoFilter()](#getAutoFilter--)| <b>@deprecated.</b> Please use the 'autoFilter' property instead. Gets the autofilter of the pivot filter. |
| [getFilterType()](#getFilterType--)| <b>@deprecated.</b> Please use the 'filterType' property instead. Gets the autofilter type of the pivot filter. |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets the index of source field which this pivot filter is applied to. |
| [getFilterCategory()](#getFilterCategory--)| <b>@deprecated.</b> Please use the 'filterCategory' property instead. Gets the category of this filter. |
| [getValue1()](#getValue1--)| <b>@deprecated.</b> Please use the 'value1' property instead. Gets the string value1 of the label pivot filter. |
| [setValue1(string)](#setValue1-string-)| <b>@deprecated.</b> Please use the 'value1' property instead. Gets the string value1 of the label pivot filter. |
| [getValue2()](#getValue2--)| <b>@deprecated.</b> Please use the 'value2' property instead. Gets the string value2 of the label pivot filter. |
| [setValue2(string)](#setValue2-string-)| <b>@deprecated.</b> Please use the 'value2' property instead. Gets the string value2 of the label pivot filter. |
| [getMeasureFldIndex()](#getMeasureFldIndex--)| <b>@deprecated.</b> Please use the 'measureFldIndex' property instead. Gets the measure field index of the pivot filter. |
| [setMeasureFldIndex(number)](#setMeasureFldIndex-number-)| <b>@deprecated.</b> Please use the 'measureFldIndex' property instead. Gets the measure field index of the pivot filter. |
| [getValueFieldIndex()](#getValueFieldIndex--)| <b>@deprecated.</b> Please use the 'valueFieldIndex' property instead. Gets the index of value field in the value region. |
| [setValueFieldIndex(number)](#setValueFieldIndex-number-)| <b>@deprecated.</b> Please use the 'valueFieldIndex' property instead. Gets the index of value field in the value region. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--)| <b>@deprecated.</b> Please use the 'measureCubeFieldIndex' property instead. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--)| <b>@deprecated.</b> Please use the 'memberPropertyFieldIndex' property instead. Gets the member property field index of the pivot filter. |
| [setMemberPropertyFieldIndex(number)](#setMemberPropertyFieldIndex-number-)| <b>@deprecated.</b> Please use the 'memberPropertyFieldIndex' property instead. Gets the member property field index of the pivot filter. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot filter. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the pivot filter. |
| [getEvaluationOrder()](#getEvaluationOrder--)| <b>@deprecated.</b> Please use the 'evaluationOrder' property instead. Gets the Evaluation Order of the pivot filter. |
| [setEvaluationOrder(number)](#setEvaluationOrder-number-)| <b>@deprecated.</b> Please use the 'evaluationOrder' property instead. Gets the Evaluation Order of the pivot filter. |
| [getTop10Value()](#getTop10Value--)| Gets top 10 setting of the filter. |
| [getLabels()](#getLabels--)| Gets labels of the caption filter. |
| [getNumberValues()](#getNumberValues--)| Gets values of the number filter. |
| [getDateTimeValues()](#getDateTimeValues--)| Gets values of the number filter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### useWholeDay {#useWholeDay--}
Indicates whether uses whole days in its filtering criteria.
```javascript
useWholeDay : boolean;
```
### autoFilter {#autoFilter--}
Readonly. Gets the autofilter of the pivot filter.
```javascript
autoFilter : AutoFilter;
```
**Remarks**
NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### filterType {#filterType--}
Readonly. Gets the autofilter type of the pivot filter.
```javascript
filterType : PivotFilterType;
```
### fieldIndex {#fieldIndex--}
Readonly. Gets the index of source field which this pivot filter is applied to.
```javascript
fieldIndex : number;
```
### filterCategory {#filterCategory--}
Readonly. Gets the category of this filter.
```javascript
filterCategory : FilterCategory;
```
### value1 {#value1--}
Gets the string value1 of the label pivot filter.
```javascript
value1 : string;
```
### value2 {#value2--}
Gets the string value2 of the label pivot filter.
```javascript
value2 : string;
```
### measureFldIndex {#measureFldIndex--}
Gets the measure field index of the pivot filter.
```javascript
measureFldIndex : number;
```
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### valueFieldIndex {#valueFieldIndex--}
Gets the index of value field in the value region.
```javascript
valueFieldIndex : number;
```
### measureCubeFieldIndex {#measureCubeFieldIndex--}
Readonly. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.
```javascript
measureCubeFieldIndex : number;
```
### memberPropertyFieldIndex {#memberPropertyFieldIndex--}
Gets the member property field index of the pivot filter.
```javascript
memberPropertyFieldIndex : number;
```
### name {#name--}
Gets the name of the pivot filter.
```javascript
name : string;
```
### evaluationOrder {#evaluationOrder--}
Gets the Evaluation Order of the pivot filter.
```javascript
evaluationOrder : number;
```
### getUseWholeDay() {#getUseWholeDay--}
```javascript
getUseWholeDay() : boolean;
```
### setUseWholeDay(boolean) {#setUseWholeDay-boolean-}
```javascript
setUseWholeDay(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAutoFilter() {#getAutoFilter--}
```javascript
getAutoFilter() : AutoFilter;
```
**Returns**
[AutoFilter](../autofilter/)
**Remarks**
NOTE: This method is now obsolete. Instead, please use FilterLabel, FilterValue,FilterDate or FilterTop10 method. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### getFilterType() {#getFilterType--}
```javascript
getFilterType() : PivotFilterType;
```
**Returns**
[PivotFilterType](../pivotfiltertype/)
### getFieldIndex() {#getFieldIndex--}
```javascript
getFieldIndex() : number;
```
### getFilterCategory() {#getFilterCategory--}
```javascript
getFilterCategory() : FilterCategory;
```
**Returns**
[FilterCategory](../filtercategory/)
### getValue1() {#getValue1--}
```javascript
getValue1() : string;
```
### setValue1(string) {#setValue1-string-}
```javascript
setValue1(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getValue2() {#getValue2--}
```javascript
getValue2() : string;
```
### setValue2(string) {#setValue2-string-}
```javascript
setValue2(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getMeasureFldIndex() {#getMeasureFldIndex--}
```javascript
getMeasureFldIndex() : number;
```
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### setMeasureFldIndex(number) {#setMeasureFldIndex-number-}
```javascript
setMeasureFldIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### getValueFieldIndex() {#getValueFieldIndex--}
```javascript
getValueFieldIndex() : number;
```
### setValueFieldIndex(number) {#setValueFieldIndex-number-}
```javascript
setValueFieldIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```javascript
getMeasureCubeFieldIndex() : number;
```
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```javascript
getMemberPropertyFieldIndex() : number;
```
### setMemberPropertyFieldIndex(number) {#setMemberPropertyFieldIndex-number-}
```javascript
setMemberPropertyFieldIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getEvaluationOrder() {#getEvaluationOrder--}
```javascript
getEvaluationOrder() : number;
```
### setEvaluationOrder(number) {#setEvaluationOrder-number-}
```javascript
setEvaluationOrder(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getTop10Value() {#getTop10Value--}
Gets top 10 setting of the filter.
```javascript
getTop10Value() : Top10Filter;
```
**Returns**
[Top10Filter](../top10filter/)
### getLabels() {#getLabels--}
Gets labels of the caption filter.
```javascript
getLabels() : string[];
```
**Returns**
string[]
### getNumberValues() {#getNumberValues--}
Gets values of the number filter.
```javascript
getNumberValues() : number[];
```
**Returns**
number[]
### getDateTimeValues() {#getDateTimeValues--}
Gets values of the number filter.
```javascript
getDateTimeValues() : Date[];
```
**Returns**
Date[]
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
