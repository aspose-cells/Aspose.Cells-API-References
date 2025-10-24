##HeaderFooterCommand
Represents the command of headerfooter
## HeaderFooterCommand class
Represents the command of header/footer
```javascript
class HeaderFooterCommand;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| HeaderFooterCommandType | Readonly. Gets the header/footer' command type . |
| [font](#font--)| Font | Readonly. Gets the font of the command's value. |
| [text](#text--)| string | Readonly. Gets the text of the command. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the header/footer' command type . |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Gets the font of the command's value. |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Gets the text of the command. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Gets the header/footer' command type .
```javascript
type : HeaderFooterCommandType;
```
### font {#font--}
Readonly. Gets the font of the command's value.
```javascript
font : Font;
```
**Remarks**
Useless for HeaderFooterCommandType.Picture.
### text {#text--}
Readonly. Gets the text of the command.
```javascript
text : string;
```
**Remarks**
Only valid for HeaderFooterCommandType.Text.
### getType() {#getType--}
```javascript
getType() : HeaderFooterCommandType;
```
**Returns**
[HeaderFooterCommandType](../headerfootercommandtype/)
### getFont() {#getFont--}
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
**Remarks**
Useless for HeaderFooterCommandType.Picture.
### getText() {#getText--}
```javascript
getText() : string;
```
**Remarks**
Only valid for HeaderFooterCommandType.Text.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
