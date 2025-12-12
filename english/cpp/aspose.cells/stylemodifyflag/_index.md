---
title: Aspose::Cells::StyleModifyFlag enum
linktitle: StyleModifyFlag
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::StyleModifyFlag enum. The style modified flags in C++.'
type: docs
weight: 26600
url: /cpp/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enum


The style modified flags.

```cpp
enum class StyleModifyFlag
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LeftBorder | 256 | <br>Indicates whether left border has been modified for the style. |
| RightBorder | 512 | <br>Indicates whether right border has been modified for the style. |
| TopBorder | 1024 | <br>Indicates whether top border has been modified for the style. |
| BottomBorder | 2048 | <br>Indicates whether bottom border has been modified for the style. |
| DiagonalDownBorder | 4096 | <br>Indicates whether diagonal-down border has been modified for the style. |
| DiagonalUpBorder | 8192 | <br>Indicates whether diagonal-up border has been modified for the style. |
| HorizontalBorder | 32 | <br>Indicates whether horizontal border has been modified for the style. Only for dynamic style, such as conditional formatting. |
| VerticalBorder | 64 | <br>Indicates whether vertical border has been modified for the style. Only for dynamic style, such as conditional formatting. |
| SideBorders | 3840 | <br>Indicates the four side borders: [LeftBorder](../bordertype/), [RightBorder](../bordertype/), [TopBorder](../bordertype/) and [BottomBorder](../bordertype/). |
| Diagonal | 12288 | <br>Indicates diagonal borders: [DiagonalDownBorder](./) and [DiagonalUpBorder](./). |
| DynamicStyleBorders | 96 | <br>Indicates borders of dynamic style: [HorizontalBorder](./) and [VerticalBorder](./). |
| Borders | 16224 | <br>Indicates whether one or more borders([LeftBorder](../bordertype/), [RightBorder](../bordertype/), [TopBorder](../bordertype/), [BottomBorder](../bordertype/), [Diagonal](../bordertype/), [HorizontalBorder](./), [VerticalBorder](./)) have been modified for the style. |
| NumberFormat | 16384 | <br>Indicates whether numberformat has been modified. |
| HorizontalAlignment | 32768 | <br>Indicates whether horizontal alignment has been modified. |
| VerticalAlignment | 65536 | <br>Indicates whether vertical alignment has been modified. |
| Indent | 131072 | <br>Indicates whether indent property has been modified. |
| Rotation | 262144 | <br>Indicates whether rotation property has been modified. |
| WrapText | 524288 | <br>Indicates whether wrap text property has been modified. |
| ShrinkToFit | 1048576 | <br>Indicates whether shrink to fit property has been modified. |
| TextDirection | 2097152 | <br>Indicates whether text direction property has been modified. |
| RelativeIndent | 128 | <br>Indicates whether relative indent property has been modified for the style. Only for dynamic style, such as conditional formatting. |
| AlignmentSettings | 4161664 | <br>Indicates whether one or more alignment-related properties([HorizontalAlignment](./), [VerticalAlignment](./), [Rotation](../../aspose.cells.drawing/shapelocktype/), [WrapText](./), [WrapText](./), [Indent](./), [ShrinkToFit](../mergedcellsshrinktype/), [TextDirection](./), [RelativeIndent](./)) have been modified. |
| Pattern | 4194304 | <br>Indicates whether pattern of the shading has been modified. |
| ForegroundColor | 8388608 | <br>Indicates whether foreground color has been modified. |
| BackgroundColor | 16777216 | <br>Indicates whether background color has been modified. |
| CellShading | 29360128 | <br>Indicates whether one or more shading-related properties([Pattern](../../aspose.cells.drawing/filltype/), [ForegroundColor](./), [BackgroundColor](../../aspose.cells.rendering/databarrendermode/)) have been modified. |
| Locked | 67108864 | <br>Indicates whether locked property has been modified. |
| HideFormula | 134217728 | <br>Indicates whether hide formula has been modified. |
| ProtectionSettings | 201326592 | <br>Indicates whether one or more protection-related properties([Locked](./), [HideFormula](./)) have been modified. |
| FontSize | 1 | <br>Indicates whether font size has been modified. |
| FontName | 2 | <br>Indicates whether font name has been modified. |
| FontColor | 3 | <br>Indicates whether font color has been modified. |
| FontWeight | 4 | <br>Indicates whether font weight has been modified. |
| FontItalic | 5 | <br>Indicates whether italic property of font has been modified. |
| FontUnderline | 6 | <br>Indicates whether underline property of font has been modified. |
| FontStrike | 7 | <br>Indicates whether strike property font has been modified. |
| FontScript | 8 | <br>Indicates whether subscript or superscript property of font has been modified. |
| FontFamily | 9 | <br>Indicates whether font family has been modified. |
| FontCharset | 10 | <br>Indicates whether charset of the font has been modified. |
| FontScheme | 11 | <br>unused. |
| FontDirty | 12 | <br>unused. |
| FontSpellingError | 13 | <br>unused. |
| FontUFillTx | 14 | <br>unused. |
| FontSpacing | 15 | <br>unused. |
| FontKerning | 16 | <br>unused. |
| FontEqualize | 17 | <br>unused. |
| FontCap | 18 | <br>unused. |
| FontVerticalText | 19 | <br> |
| Font | 31 | <br>Indicates whether one or more properties have been modified for the font of the style. |
| All | 234881023 | <br>All properties that can be modified for the style. |
| None | 0 | <br>No property has been specified. |

## Remarks


Combinations of multiple properties are defined for user's convenience. When checking whether they are modified for one style, the returned value denotes whether one or more properties in the combination have been modified. 
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
