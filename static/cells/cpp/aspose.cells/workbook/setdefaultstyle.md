##Aspose::Cells::Workbook::SetDefaultStyle method
'Aspose::Cells::Workbook::SetDefaultStyle method. Gets or sets the default Style object of the workbook in C++.'
## Workbook::SetDefaultStyle method
Gets or sets the default [Style](../../style/) object of the workbook.
```cpp
void Aspose::Cells::Workbook::SetDefaultStyle(const Style &value)
```
## Remarks
The DefaultStyle property is useful to implement a [Style](../../style/) for the whole [Workbook](../).
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
Style defaultStyle = workbook.GetDefaultStyle();
defaultStyle.GetFont().SetName(u"Tahoma");
workbook.SetDefaultStyle(defaultStyle);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [Style](../../style/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
