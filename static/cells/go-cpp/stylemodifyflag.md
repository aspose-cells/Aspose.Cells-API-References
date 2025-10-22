##StyleModifyFlag Enum
'StyleModifyFlag enum. Encapsulates the object that represents stylemodifyflag in Go.'
## StyleModifyFlag Enum
The style modified flags.
```go
type StyleModifyFlag int32
```
## Fields
| Field | Description |
| --- | --- |
|[LeftBorder](./leftborder/) | Indicates whether left border has been modified for the style. |
|[RightBorder](./rightborder/) | Indicates whether right border has been modified for the style. |
|[TopBorder](./topborder/) | Indicates whether top border has been modified for the style. |
|[BottomBorder](./bottomborder/) | Indicates whether bottom border has been modified for the style. |
|[DiagonalDownBorder](./diagonaldownborder/) | Indicates whether diagonal-down border has been modified for the style. |
|[DiagonalUpBorder](./diagonalupborder/) | Indicates whether diagonal-up border has been modified for the style. |
|[HorizontalBorder](./horizontalborder/) | Indicates whether horizontal border has been modified for the style.Only for dynamic style, such as conditional formatting. |
|[VerticalBorder](./verticalborder/) | Indicates whether vertical border has been modified for the style.Only for dynamic style, such as conditional formatting. |
|[SideBorders](./sideborders/) | Indicates the four side borders: <see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/> and <see cref="BottomBorder"/>. |
|[Diagonal](./diagonal/) | Indicates diagonal borders: <see cref="DiagonalDownBorder"/> and <see cref="DiagonalUpBorder"/>. |
|[DynamicStyleBorders](./dynamicstyleborders/) | Indicates borders of dynamic style: <see cref="HorizontalBorder"/> and <see cref="VerticalBorder"/>. |
|[Borders](./borders/) | Indicates whether one or more borders(<see cref="LeftBorder"/>,<see cref="RightBorder"/>, <see cref="TopBorder"/>, <see cref="BottomBorder"/>,<see cref="Diagonal"/>, <see cref="HorizontalBorder"/>, <see cref="VerticalBorder"/>)have been modified for the style. |
|[NumberFormat](./numberformat/) | Indicates whether numberformat has been modified. |
|[HorizontalAlignment](./horizontalalignment/) | Indicates whether horizontal alignment has been modified. |
|[VerticalAlignment](./verticalalignment/) | Indicates whether vertical alignment has been modified. |
|[Indent](./indent/) | Indicates whether indent property has been modified. |
|[Rotation](./rotation/) | Indicates whether rotation property has been modified. |
|[WrapText](./wraptext/) | Indicates whether wrap text property has been modified. |
|[ShrinkToFit](./shrinktofit/) | Indicates whether shrink to fit property has been modified. |
|[TextDirection](./textdirection/) | Indicates whether text direction property has been modified. |
|[RelativeIndent](./relativeindent/) | Indicates whether relative indent property has been modified for the style.Only for dynamic style, such as conditional formatting. |
|[AlignmentSettings](./alignmentsettings/) | Indicates whether one or more alignment-related properties(<see cref="HorizontalAlignment"/>,<see cref="VerticalAlignment"/>, <see cref="Rotation"/>, <see cref="WrapText"/>,<see cref="WrapText"/>, <see cref="Indent"/>, <see cref="ShrinkToFit"/>, <see cref="TextDirection"/>,<see cref="RelativeIndent"/>) have been modified. |
|[Pattern](./pattern/) | Indicates whether pattern of the shading has been modified. |
|[ForegroundColor](./foregroundcolor/) | Indicates whether foreground color has been modified. |
|[BackgroundColor](./backgroundcolor/) | Indicates whether background color has been modified. |
|[CellShading](./cellshading/) | Indicates whether one or more shading-related properties(<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>) have been modified. |
|[Locked](./locked/) | Indicates whether locked property has been modified. |
|[HideFormula](./hideformula/) | Indicates whether hide formula has been modified. |
|[ProtectionSettings](./protectionsettings/) | Indicates whether one or more protection-related properties(<see cref="Locked"/>,<see cref="HideFormula"/>) have been modified. |
|[FontSize](./fontsize/) | Indicates whether font size has been modified. |
|[FontName](./fontname/) | Indicates whether font name has been modified. |
|[FontColor](./fontcolor/) | Indicates whether font color has been modified. |
|[FontWeight](./fontweight/) | Indicates whether font weight has been modified. |
|[FontItalic](./fontitalic/) | Indicates whether italic property of font has been modified. |
|[FontUnderline](./fontunderline/) | Indicates whether underline property of font has been modified. |
|[FontStrike](./fontstrike/) | Indicates whether strike property font has been modified. |
|[FontScript](./fontscript/) | Indicates whether subscript or superscript property of font has been modified. |
|[FontFamily](./fontfamily/) | Indicates whether font family has been modified. |
|[FontCharset](./fontcharset/) | Indicates whether charset of the font has been modified. |
|[FontScheme](./fontscheme/) | unused. |
|[FontDirty](./fontdirty/) | unused. |
|[FontSpellingError](./fontspellingerror/) | unused. |
|[FontUFillTx](./fontufilltx/) | unused. |
|[FontSpacing](./fontspacing/) | unused. |
|[FontKerning](./fontkerning/) | unused. |
|[FontEqualize](./fontequalize/) | unused. |
|[FontCap](./fontcap/) | unused. |
|[FontVerticalText](./fontverticaltext/) |  |
|[Font](./font/) | Indicates whether one or more properties have been modified for the font of the style. |
|[All](./all/) | All properties that can be modified for the style. |
|[None](./none/) | No property has been specified. |
