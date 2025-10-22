##Aspose::Cells::ThemeColor class
'Aspose::Cells::ThemeColor class. Represents a theme color in C++.'
## ThemeColor class
Represents a theme color.
```cpp
class ThemeColor
```
## Methods
| Method | Description |
| --- | --- |
| [GetColorType()](./getcolortype/) | Gets and sets the theme type. |
| [GetTint()](./gettint/) | Gets and sets the tint value. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ThemeColor\& src)](./operator_asm/) | operator= |
| [SetColorType(ThemeColorType value)](./setcolortype/) | Gets and sets the theme type. |
| [SetTint(double value)](./settint/) | Gets and sets the tint value. |
| [ThemeColor(ThemeColorType type, double tint)](./themecolor/) |  |
| [ThemeColor(ThemeColor_Impl* impl)](./themecolor/) | Constructs from an implementation object. |
| [ThemeColor(const ThemeColor\& src)](./themecolor/) | Copy constructor. |
| [~ThemeColor()](./~themecolor/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").PutValue(u"Hello World");
Style style = cells.Get(u"A1").GetStyle();
//Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.GetFont().SetThemeColor(ThemeColor(ThemeColorType::Text2, 0.4));
style.SetPattern(BackgroundType::Solid);
//Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.SetForegroundThemeColor(ThemeColor(ThemeColorType::Background2, -0.75));
cells.Get(u"A1").SetStyle(style);
//Saving the Excel file
workbook.Save(u"book1.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
