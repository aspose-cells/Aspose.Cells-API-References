##Aspose::Cells::Cell::Characters method
'Aspose::Cells::Cell::Characters method. Returns a Characters object that represents a range of characters within the cell text in C++.'
## Cell::Characters method
Returns a Characters object that represents a range of characters within the cell text.
```cpp
FontSetting Aspose::Cells::Cell::Characters(int32_t startIndex, int32_t length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int32_t | The index of the start of the character. |
| length | int32_t | The number of characters. |
## ReturnValue
Characters object.
## Remarks
This method only works on cell with string value.
## Examples
```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").PutValue(u"Helloworld");
cells.Get(u"A1").Characters(5, 5).GetFont().SetIsBold(true);
cells.Get(u"A1").Characters(5, 5).GetFont().SetColor(Color{ 0xff, 0, 0, 0xff });
Aspose::Cells::Cleanup();
```
## See Also
* Class [FontSetting](../../fontsetting/)
* Class [Vector](../../vector/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
