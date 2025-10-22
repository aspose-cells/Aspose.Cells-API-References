##PivotShowValuesSetting
Represents the settings about showing values as when the ShowDataAs calculation is in use.
## PivotShowValuesSetting class
Represents the settings about showing values as when the ShowDataAs calculation is in use.
```javascript
class PivotShowValuesSetting;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [calculationType](#calculationType--)| PivotFieldDataDisplayFormat | Represents how to show values of a data field in the pivot report. |
| [baseFieldIndex](#baseFieldIndex--)| number | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [baseItemPositionType](#baseItemPositionType--)| PivotItemPositionType | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [baseItemIndex](#baseItemIndex--)| number | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
## Methods
| Method | Description |
| --- | --- |
| [getCalculationType()](#getCalculationType--)| <b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report. |
| [setCalculationType(PivotFieldDataDisplayFormat)](#setCalculationType-pivotfielddatadisplayformat-)| <b>@deprecated.</b> Please use the 'calculationType' property instead. Represents how to show values of a data field in the pivot report. |
| [getBaseFieldIndex()](#getBaseFieldIndex--)| <b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [setBaseFieldIndex(number)](#setBaseFieldIndex-number-)| <b>@deprecated.</b> Please use the 'baseFieldIndex' property instead. Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [getBaseItemPositionType()](#getBaseItemPositionType--)| <b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [setBaseItemPositionType(PivotItemPositionType)](#setBaseItemPositionType-pivotitempositiontype-)| <b>@deprecated.</b> Please use the 'baseItemPositionType' property instead. Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. |
| [getBaseItemIndex()](#getBaseItemIndex--)| <b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [setBaseItemIndex(number)](#setBaseItemIndex-number-)| <b>@deprecated.</b> Please use the 'baseItemIndex' property instead. Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### calculationType {#calculationType--}
Represents how to show values of a data field in the pivot report.
```javascript
calculationType : PivotFieldDataDisplayFormat;
```
### baseFieldIndex {#baseFieldIndex--}
Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.
```javascript
baseFieldIndex : number;
```
### baseItemPositionType {#baseItemPositionType--}
Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute.
```javascript
baseItemPositionType : PivotItemPositionType;
```
### baseItemIndex {#baseItemIndex--}
Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.
```javascript
baseItemIndex : number;
```
### getCalculationType() {#getCalculationType--}
```javascript
getCalculationType() : PivotFieldDataDisplayFormat;
```
**Returns**
[PivotFieldDataDisplayFormat](../pivotfielddatadisplayformat/)
### setCalculationType(PivotFieldDataDisplayFormat) {#setCalculationType-pivotfielddatadisplayformat-}
```javascript
setCalculationType(value: PivotFieldDataDisplayFormat) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldDataDisplayFormat](../pivotfielddatadisplayformat/) | The value to set. |
### getBaseFieldIndex() {#getBaseFieldIndex--}
```javascript
getBaseFieldIndex() : number;
```
### setBaseFieldIndex(number) {#setBaseFieldIndex-number-}
```javascript
setBaseFieldIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBaseItemPositionType() {#getBaseItemPositionType--}
```javascript
getBaseItemPositionType() : PivotItemPositionType;
```
**Returns**
[PivotItemPositionType](../pivotitempositiontype/)
### setBaseItemPositionType(PivotItemPositionType) {#setBaseItemPositionType-pivotitempositiontype-}
```javascript
setBaseItemPositionType(value: PivotItemPositionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotItemPositionType](../pivotitempositiontype/) | The value to set. |
### getBaseItemIndex() {#getBaseItemIndex--}
```javascript
getBaseItemIndex() : number;
```
### setBaseItemIndex(number) {#setBaseItemIndex-number-}
```javascript
setBaseItemIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
