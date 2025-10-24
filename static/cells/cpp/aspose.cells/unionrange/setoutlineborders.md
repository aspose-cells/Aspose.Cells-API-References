##Aspose::Cells::UnionRange::SetOutlineBorders method
'Aspose::Cells::UnionRange::SetOutlineBorders method. Sets out line borders around a range of cells in C++.'
## UnionRange::SetOutlineBorders(const Vector \<CellBorderType\>\&, const Vector \<Aspose::Cells::Color\>\&) method
Sets out line borders around a range of cells.
```cpp
void Aspose::Cells::UnionRange::SetOutlineBorders(const Vector<CellBorderType> &borderStyles, const Vector<Aspose::Cells::Color> &borderColors)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | const Vector \<CellBorderType\>\& | [Border](../../border/) styles. |
| borderColors | const Vector \<Aspose::Cells::Color\>\& | [Border](../../border/) colors. |
## Remarks
Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right
## See Also
* Class [Vector](../../vector/)
* Enum [CellBorderType](../../cellbordertype/)
* Class [UnionRange](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## UnionRange::SetOutlineBorders(CellBorderType, const Aspose::Cells::Color\&) method
Sets the outline borders around a range of cells with same border style and color.
```cpp
void Aspose::Cells::UnionRange::SetOutlineBorders(CellBorderType borderStyle, const Aspose::Cells::Color &borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | [Border](../../border/) style. |
| borderColor | const Aspose::Cells::Color\& | [Border](../../border/) color. |
## See Also
* Class [Vector](../../vector/)
* Enum [CellBorderType](../../cellbordertype/)
* Class [UnionRange](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
