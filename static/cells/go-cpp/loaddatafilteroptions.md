##LoadDataFilterOptions Enum
'LoadDataFilterOptions enum. Encapsulates the object that represents loaddatafilteroptions in Go.'
## LoadDataFilterOptions Enum
Represents the options to filter data when loading workbook from template.
```go
type LoadDataFilterOptions int32
```
## Fields
| Field | Description |
| --- | --- |
|[All](./all/) | Load all |
|[CellBlank](./cellblank/) | Load cells whose value is blank |
|[CellString](./cellstring/) | Load cells whose value is string |
|[CellNumeric](./cellnumeric/) | Load cells whose value is numeric(including datetime) |
|[CellError](./cellerror/) | Load cells whose value is error |
|[CellBool](./cellbool/) | Load cells whose value is bool |
|[CellValue](./cellvalue/) | Load cells value(all value types) only |
|[Formula](./formula/) | Load cell formulas. |
|[CellData](./celldata/) | Load cells data including values, formulas and formatting |
|[Chart](./chart/) | Load charts |
|[Drawing](./drawing/) | Drawing objects(including Chart, Picture, OleObject and all other drawing objects) |
|[MergedArea](./mergedarea/) | Load merged cells |
|[ConditionalFormatting](./conditionalformatting/) | Load conditional formatting |
|[DataValidation](./datavalidation/) | Load data validations |
|[PivotTable](./pivottable/) | Load pivot tables |
|[Table](./table/) | Load tables |
|[Hyperlinks](./hyperlinks/) | Load hyperlinks |
|[SheetSettings](./sheetsettings/) | Load settings for worksheet |
|[SheetData](./sheetdata/) | Load all data of worksheet, such as cells data, settings, objects, ...etc. |
|[BookSettings](./booksettings/) | Load settings for workbook |
|[Settings](./settings/) | Load settings for workbook and worksheet |
|[XmlMap](./xmlmap/) | Load XmlMap |
|[Structure](./structure/) | Load structure of the workbook |
|[Document_Properties](./document_properties/) | Load document properties |
|[DefinedNames](./definednames/) | Load defined Name objects |
|[VBA](./vba/) | Load VBA projects |
|[Style](./style/) | Load styles for cell formatting |
|[Picture](./picture/) | Load pictures |
|[OleObject](./oleobject/) | Load OleObjects |
|[Revision](./revision/) | Load revision logs |
