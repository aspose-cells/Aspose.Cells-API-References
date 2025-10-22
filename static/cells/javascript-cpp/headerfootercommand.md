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
