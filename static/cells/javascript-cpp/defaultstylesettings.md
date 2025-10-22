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
