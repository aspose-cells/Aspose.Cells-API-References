##StyleModifyFlag
The style modified flags.
## StyleModifyFlag enumeration
The style modified flags.
### Remarks
Combinations of multiple properties are defined for user's convenience. When checking whether they are modified for one style, the returned value denotes whether one or more properties in the combination have been modified.
### Values
| Name | Value | Description |
| --- | --- | --- |
| LeftBorder | `256` | Indicates whether left border has been modified for the style. |
| RightBorder | `512` | Indicates whether right border has been modified for the style. |
| TopBorder | `1024` | Indicates whether top border has been modified for the style. |
| BottomBorder | `2048` | Indicates whether bottom border has been modified for the style. |
| DiagonalDownBorder | `4096` | Indicates whether diagonal-down border has been modified for the style. |
| DiagonalUpBorder | `8192` | Indicates whether diagonal-up border has been modified for the style. |
| HorizontalBorder | `32` | Indicates whether horizontal border has been modified for the style. Only for dynamic style, such as conditional formatting. |
| VerticalBorder | `64` | Indicates whether vertical border has been modified for the style. Only for dynamic style, such as conditional formatting. |
| SideBorders | `3840` | Indicates the four side borders: [LeftBorder](../leftborder/), [RightBorder](../rightborder/), [TopBorder](../topborder/) and [BottomBorder](../bottomborder/). |
| Diagonal | `12288` | Indicates diagonal borders: [DiagonalDownBorder](../diagonaldownborder/) and [DiagonalUpBorder](../diagonalupborder/). |
| DynamicStyleBorders | `96` | Indicates borders of dynamic style: [HorizontalBorder](../horizontalborder/) and [VerticalBorder](../verticalborder/). |
| Borders | `16224` | Indicates whether one or more borders([LeftBorder](../leftborder/), [RightBorder](../rightborder/), [TopBorder](../topborder/), [BottomBorder](../bottomborder/), [Diagonal](../diagonal/), [HorizontalBorder](../horizontalborder/), [VerticalBorder](../verticalborder/)) have been modified for the style. |
| NumberFormat | `16384` | Indicates whether numberformat has been modified. |
| HorizontalAlignment | `32768` | Indicates whether horizontal alignment has been modified. |
| VerticalAlignment | `65536` | Indicates whether vertical alignment has been modified. |
| Indent | `131072` | Indicates whether indent property has been modified. |
| Rotation | `262144` | Indicates whether rotation property has been modified. |
| WrapText | `524288` | Indicates whether wrap text property has been modified. |
| ShrinkToFit | `1048576` | Indicates whether shrink to fit property has been modified. |
| TextDirection | `2097152` | Indicates whether text direction property has been modified. |
| RelativeIndent | `128` | Indicates whether relative indent property has been modified for the style. Only for dynamic style, such as conditional formatting. |
| AlignmentSettings | `4161664` | Indicates whether one or more alignment-related properties([HorizontalAlignment](../horizontalalignment/), [VerticalAlignment](../verticalalignment/), [Rotation](../rotation/), [WrapText](../wraptext/), [WrapText](../wraptext/), [Indent](../indent/), [ShrinkToFit](../shrinktofit/), [TextDirection](../textdirection/), [RelativeIndent](../relativeindent/)) have been modified. |
| Pattern | `4194304` | Indicates whether pattern of the shading has been modified. |
| ForegroundColor | `8388608` | Indicates whether foreground color has been modified. |
| BackgroundColor | `16777216` | Indicates whether background color has been modified. |
| CellShading | `29360128` | Indicates whether one or more shading-related properties([Pattern](../pattern/), [ForegroundColor](../foregroundcolor/), [BackgroundColor](../backgroundcolor/)) have been modified. |
| Locked | `67108864` | Indicates whether locked property has been modified. |
| HideFormula | `134217728` | Indicates whether hide formula has been modified. |
| ProtectionSettings | `201326592` | Indicates whether one or more protection-related properties([Locked](../locked/), [HideFormula](../hideformula/)) have been modified. |
| FontSize | `1` | Indicates whether font size has been modified. |
| FontName | `2` | Indicates whether font name has been modified. |
| FontColor | `3` | Indicates whether font color has been modified. |
| FontWeight | `4` | Indicates whether font weight has been modified. |
| FontItalic | `5` | Indicates whether italic property of font has been modified. |
| FontUnderline | `6` | Indicates whether underline property of font has been modified. |
| FontStrike | `7` | Indicates whether strike property font has been modified. |
| FontScript | `8` | Indicates whether subscript or superscript property of font has been modified. |
| FontFamily | `9` | Indicates whether font family has been modified. |
| FontCharset | `10` | Indicates whether charset of the font has been modified. |
| FontScheme | `11` | unused. |
| FontDirty | `12` | unused. |
| FontSpellingError | `13` | unused. |
| FontUFillTx | `14` | unused. |
| FontSpacing | `15` | unused. |
| FontKerning | `16` | unused. |
| FontEqualize | `17` | unused. |
| FontCap | `18` | unused. |
| FontVerticalText | `19` |  |
| Font | `31` | Indicates whether one or more properties have been modified for the font of the style. |
| All | `234881023` | All properties that can be modified for the style. |
| None | `0` | No property has been specified. |
