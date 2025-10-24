##Aspose::Cells::LoadDataFilterOptions enum
'Aspose::Cells::LoadDataFilterOptions enum. Represents the options to filter data when loading workbook from template in C++.'
## LoadDataFilterOptions enum
Represents the options to filter data when loading workbook from template.
```cpp
enum class LoadDataFilterOptions
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | 0 |  **(Deprecated - Use Structure instead. )** <br>Load nothing for sheet data. |
| All | 2147483647 | <br>Load all. |
| CellBlank | 1 | <br>Load cells whose value is blank. |
| CellString | 2 | <br>Load cells whose value is string. |
| CellNumeric | 4 | <br>Load cells whose value is numeric(including datetime) |
| CellError | 8 | <br>Load cells whose value is error. |
| CellBool | 16 | <br>Load cells whose value is bool. |
| CellValue | 31 | <br>Load cells value(all value types) only. |
| Formula | 32 | <br>Load cell formulas. |
| CellData | 67108927 | <br>Load cells data including values, formulas and formatting. |
| Chart | 256 | <br>Load charts. |
| Shape | 402653696 |  **(Deprecated - Use Drawing instead. )** <br>Load shapes. |
| Drawing | 402653952 | <br>[Drawing](../../aspose.cells.drawing/) objects(including Chart, Picture, OleObject and all other drawing objects) |
| MergedArea | 1024 | <br>Load merged cells. |
| ConditionalFormatting | 2048 | <br>Load conditional formatting. |
| DataValidation | 4096 | <br>Load data validations. |
| PivotTable | 8192 | <br>Load pivot tables. |
| Table | 16384 | <br>Load tables. |
| Hyperlinks | 32768 | <br>Load hyperlinks. |
| SheetSettings | 65536 | <br>Load settings for worksheet. |
| SheetData | 403701759 | <br>Load all data of worksheet, such as cells data, settings, objects, ...etc. |
| BookSettings | 1048576 | <br>Load settings for workbook. |
| Settings | 1114112 | <br>Load settings for workbook and worksheet. |
| XmlMap | 2097152 | <br>Load [XmlMap](../xmlmap/). |
| Structure | 4194304 | <br>Load structure of the workbook. |
| Document_Properties | 8388608 | <br>Load document properties. |
| DefinedNames | 16777216 | <br>Load defined [Name](../name/) objects. |
| VBA | 33554432 | <br>Load VBA projects. |
| Style | 67108864 | <br>Load styles for cell formatting. |
| Picture | 134217728 | <br>Load pictures. |
| OleObject | 268435456 | <br>Load OleObjects. |
| Revision | 536870912 | <br>Load revision logs. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
