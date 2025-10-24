##JsonLayoutOptions
Represents the options of json layout type.
## JsonLayoutOptions class
Represents the options of json layout type.
```javascript
class JsonLayoutOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructor of loading JSON layout options. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [arrayAsTable](#arrayAsTable--)| boolean | Processes Array as table. |
| [ignoreNull](#ignoreNull--)| boolean | Indicates whether ignoring null value. |
| [ignoreTitle](#ignoreTitle--)| boolean | Ingores titles of attributes |
| [convertNumericOrDate](#convertNumericOrDate--)| boolean | Indicates whether converting the string in json to numeric or date value. |
| [numberFormat](#numberFormat--)| string | Gets and sets the format of numeric value. |
| [dateFormat](#dateFormat--)| string | Gets and sets the format of date value. |
| [titleStyle](#titleStyle--)| Style | Gets and sets the style of the title. |
| [keptSchema](#keptSchema--)| boolean | Indicates whether keeping schema of this json. |
### constructor() {#constructor--}
Constructor of loading JSON layout options.
```javascript
constructor();
```
### arrayAsTable {#arrayAsTable--}
Processes Array as table.
```javascript
arrayAsTable : boolean;
```
### ignoreNull {#ignoreNull--}
Indicates whether ignoring null value.
```javascript
ignoreNull : boolean;
```
### ignoreTitle {#ignoreTitle--}
Ingores titles of attributes
```javascript
ignoreTitle : boolean;
```
### convertNumericOrDate {#convertNumericOrDate--}
Indicates whether converting the string in json to numeric or date value.
```javascript
convertNumericOrDate : boolean;
```
### numberFormat {#numberFormat--}
Gets and sets the format of numeric value.
```javascript
numberFormat : string;
```
### dateFormat {#dateFormat--}
Gets and sets the format of date value.
```javascript
dateFormat : string;
```
### titleStyle {#titleStyle--}
Gets and sets the style of the title.
```javascript
titleStyle : Style;
```
### keptSchema {#keptSchema--}
Indicates whether keeping schema of this json.
```javascript
keptSchema : boolean;
```
**Remarks**
Sometimes we will save the file to JSON after loading JSON file.
