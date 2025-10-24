##Aspose::Cells::BorderCollection class
'Aspose::Cells::BorderCollection class. Encapsulates a collection of Border objects in C++.'
## BorderCollection class
Encapsulates a collection of [Border](../border/) objects.
```cpp
class BorderCollection
```
## Methods
| Method | Description |
| --- | --- |
| [BorderCollection(BorderCollection_Impl* impl)](./bordercollection/) | Constructs from an implementation object. |
| [BorderCollection(const BorderCollection\& src)](./bordercollection/) | Copy constructor. |
| [Get(BorderType borderType)](./get/) | Gets the [Border](../border/) element at the specified index. |
| [GetDiagonalColor()](./getdiagonalcolor/) | Gets or sets the [Color](../color/) of Diagonal lines. |
| [GetDiagonalStyle()](./getdiagonalstyle/) | Gets or sets the style of Diagonal lines. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const BorderCollection\& src)](./operator_asm/) | operator= |
| [SetColor(const Aspose::Cells::Color\& color)](./setcolor/) | Sets the [Color](../color/) of all borders in the collection. |
| [SetDiagonalColor(const Aspose::Cells::Color\& value)](./setdiagonalcolor/) | Gets or sets the [Color](../color/) of Diagonal lines. |
| [SetDiagonalStyle(CellBorderType value)](./setdiagonalstyle/) | Gets or sets the style of Diagonal lines. |
| [SetStyle(CellBorderType style)](./setstyle/) | Sets the style of all borders of the collection. |
| [~BorderCollection()](./~bordercollection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
//Adding a new worksheet to the Excel object
workbook.GetWorksheets().Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Accessing the "A1" cell from the worksheet
Cell cell = worksheet.GetCells().Get(u"A1");
//Adding some value to the "A1" cell
cell.PutValue(u"Visit Aspose!");
Style style = cell.GetStyle();
//Setting the line style of the top border
style.GetBorders().Get(BorderType::TopBorder).SetLineStyle(CellBorderType::Thick);
//Setting the color of the top border
style.GetBorders().Get(BorderType::TopBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black
//Setting the line style of the bottom border
style.GetBorders().Get(BorderType::BottomBorder).SetLineStyle(CellBorderType::Thick);
//Setting the color of the bottom border
style.GetBorders().Get(BorderType::BottomBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black
//Setting the line style of the left border
style.GetBorders().Get(BorderType::LeftBorder).SetLineStyle(CellBorderType::Thick);
//Setting the color of the left border
style.GetBorders().Get(BorderType::LeftBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black
//Setting the line style of the right border
style.GetBorders().Get(BorderType::RightBorder).SetLineStyle(CellBorderType::Thick);
//Setting the color of the right border
style.GetBorders().Get(BorderType::RightBorder).SetColor(Color{ 0xff, 0, 0, 0 });//Black
cell.SetStyle(style);
//Saving the Excel file
workbook.Save(u"book1.xls");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
