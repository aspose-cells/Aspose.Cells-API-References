##DefaultStyleSettings
Settings for the default values of workbooks style properties.
## DefaultStyleSettings class
Settings for the default values of workbook's style properties.
```javascript
class DefaultStyleSettings;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [builtInPreference](#builtInPreference--)| boolean | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [fontName](#fontName--)| string | Gets/Sets the default font name for the workbook |
| [fontSize](#fontSize--)| number | Gets/Sets the default standard font size for the workbook. |
| [horizontalAlignment](#horizontalAlignment--)| TextAlignmentType | Gets/Sets the default value for horizontal alignment |
| [verticalAlignment](#verticalAlignment--)| TextAlignmentType | Gets/Sets the default value for vertical alignment |
## Methods
| Method | Description |
| --- | --- |
| [getBuiltInPreference()](#getBuiltInPreference--)| <b>@deprecated.</b> Please use the 'builtInPreference' property instead. Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [setBuiltInPreference(boolean)](#setBuiltInPreference-boolean-)| <b>@deprecated.</b> Please use the 'builtInPreference' property instead. Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. |
| [getFontName()](#getFontName--)| <b>@deprecated.</b> Please use the 'fontName' property instead. Gets/Sets the default font name for the workbook |
| [setFontName(string)](#setFontName-string-)| <b>@deprecated.</b> Please use the 'fontName' property instead. Gets/Sets the default font name for the workbook |
| [getFontSize()](#getFontSize--)| <b>@deprecated.</b> Please use the 'fontSize' property instead. Gets/Sets the default standard font size for the workbook. |
| [setFontSize(number)](#setFontSize-number-)| <b>@deprecated.</b> Please use the 'fontSize' property instead. Gets/Sets the default standard font size for the workbook. |
| [getHorizontalAlignment()](#getHorizontalAlignment--)| <b>@deprecated.</b> Please use the 'horizontalAlignment' property instead. Gets/Sets the default value for horizontal alignment |
| [setHorizontalAlignment(TextAlignmentType)](#setHorizontalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'horizontalAlignment' property instead. Gets/Sets the default value for horizontal alignment |
| [getVerticalAlignment()](#getVerticalAlignment--)| <b>@deprecated.</b> Please use the 'verticalAlignment' property instead. Gets/Sets the default value for vertical alignment |
| [setVerticalAlignment(TextAlignmentType)](#setVerticalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'verticalAlignment' property instead. Gets/Sets the default value for vertical alignment |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### builtInPreference {#builtInPreference--}
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
```javascript
builtInPreference : boolean;
```
**Remarks**
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
### fontName {#fontName--}
Gets/Sets the default font name for the workbook
```javascript
fontName : string;
```
### fontSize {#fontSize--}
Gets/Sets the default standard font size for the workbook.
```javascript
fontSize : number;
```
### horizontalAlignment {#horizontalAlignment--}
Gets/Sets the default value for horizontal alignment
```javascript
horizontalAlignment : TextAlignmentType;
```
### verticalAlignment {#verticalAlignment--}
Gets/Sets the default value for vertical alignment
```javascript
verticalAlignment : TextAlignmentType;
```
### getBuiltInPreference() {#getBuiltInPreference--}
```javascript
getBuiltInPreference() : boolean;
```
**Remarks**
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
### setBuiltInPreference(boolean) {#setBuiltInPreference-boolean-}
```javascript
setBuiltInPreference(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
### getFontName() {#getFontName--}
```javascript
getFontName() : string;
```
### setFontName(string) {#setFontName-string-}
```javascript
setFontName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getFontSize() {#getFontSize--}
```javascript
getFontSize() : number;
```
### setFontSize(number) {#setFontSize-number-}
```javascript
setFontSize(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHorizontalAlignment() {#getHorizontalAlignment--}
```javascript
getHorizontalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setHorizontalAlignment(TextAlignmentType) {#setHorizontalAlignment-textalignmenttype-}
```javascript
setHorizontalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getVerticalAlignment() {#getVerticalAlignment--}
```javascript
getVerticalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setVerticalAlignment(TextAlignmentType) {#setVerticalAlignment-textalignmenttype-}
```javascript
setVerticalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
