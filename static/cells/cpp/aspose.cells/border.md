##Aspose::Cells::Border class
'Aspose::Cells::Border class. Encapsulates the object that represents the cell border in C++.'
## Border class
Encapsulates the object that represents the cell border.
```cpp
class Border
```
## Methods
| Method | Description |
| --- | --- |
| [Border(Border_Impl* impl)](./border/) | Constructs from an implementation object. |
| [Border(const Border\& src)](./border/) | Copy constructor. |
| [GetArgbColor()](./getargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
| [GetColor()](./getcolor/) | Gets or sets the [Color](../color/) of the border. |
| [GetLineStyle()](./getlinestyle/) | Gets or sets the cell border type. |
| [GetThemeColor()](./getthemecolor/) | Gets and sets the theme color of the border. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Border\& src)](./operator_asm/) | operator= |
| [SetArgbColor(int32_t value)](./setargbcolor/) | Gets and sets the color with a 32-bit ARGB value. |
| [SetColor(const Aspose::Cells::Color\& value)](./setcolor/) | Gets or sets the [Color](../color/) of the border. |
| [SetLineStyle(CellBorderType value)](./setlinestyle/) | Gets or sets the cell border type. |
| [SetThemeColor(const ThemeColor\& value)](./setthemecolor/) | Gets and sets the theme color of the border. |
| [~Border()](./~border/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
WorksheetCollection sheets = workbook.GetWorksheets();
Cell cell = sheets.Get(0).GetCells().Get(u"A1");
Style style = cell.GetStyle();
//Set top border style and color
Border border = style.GetBorders().Get(BorderType::TopBorder);
border.SetLineStyle(CellBorderType::Medium);
border.SetColor(Color{ 0xff, 0xff, 0, 0 });//Red
cell.SetStyle(style);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
