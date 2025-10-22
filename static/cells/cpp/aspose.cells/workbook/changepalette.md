##Aspose::Cells::Workbook::ChangePalette method
'Aspose::Cells::Workbook::ChangePalette method. Changes the palette for the spreadsheet in the specified index in C++.'
## Workbook::ChangePalette method
Changes the palette for the spreadsheet in the specified index.
```cpp
void Aspose::Cells::Workbook::ChangePalette(const Aspose::Cells::Color &color, int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | const Aspose::Cells::Color\& | [Color](../../color/) structure. |
| index | int32_t | Palette index, 0 - 55. |
## Remarks
The palette has 56 entries, each represented by an RGB value.
If you set a color which is not in the palette, it will not take effect.
So if you want to set a custom color, please change the palette at first.
The following is the standard color palette.
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
