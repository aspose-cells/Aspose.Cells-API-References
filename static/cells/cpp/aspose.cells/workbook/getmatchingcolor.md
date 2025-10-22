##Aspose::Cells::Workbook::GetMatchingColor method
'Aspose::Cells::Workbook::GetMatchingColor method. Find best matching Color in current palette in C++.'
## Workbook::GetMatchingColor method
Find best matching [Color](../../color/) in current palette.
```cpp
Aspose::Cells::Color Aspose::Cells::Workbook::GetMatchingColor(const Aspose::Cells::Color &rawColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rawColor | const Aspose::Cells::Color\& | Raw color. |
## ReturnValue
Best matching color.
## Remarks
There are only 56 colors in the color palette in Excel 97-2003. If the color is not in the palette, the similar color will be set.
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
