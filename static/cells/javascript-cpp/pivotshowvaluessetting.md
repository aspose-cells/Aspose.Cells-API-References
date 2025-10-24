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
