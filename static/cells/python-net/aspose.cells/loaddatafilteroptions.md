##LoadDataFilterOptions enumeration
## LoadDataFilterOptions enumeration
Represents the options to filter data when loading workbook from template.
The LoadDataFilterOptions type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| NONE | Load nothing for sheet data |
| ALL | Load all |
| CELL_BLANK | Load cells whose value is blank |
| CELL_STRING | Load cells whose value is string |
| CELL_NUMERIC | Load cells whose value is numeric(including datetime) |
| CELL_ERROR | Load cells whose value is error |
| CELL_BOOL | Load cells whose value is bool |
| CELL_VALUE | Load cells value(all value types) only |
| FORMULA | Load cell formulas. |
| CELL_DATA | Load cells data including values, formulas and formatting |
| CHART | Load charts |
| SHAPE | Load shapes |
| DRAWING | Drawing objects(including Chart, Picture, OleObject and all other drawing objects) |
| MERGED_AREA | Load merged cells |
| CONDITIONAL_FORMATTING | Load conditional formatting |
| DATA_VALIDATION | Load data validations |
| PIVOT_TABLE | Load pivot tables |
| TABLE | Load tables |
| HYPERLINKS | Load hyperlinks |
| SHEET_SETTINGS | Load settings for worksheet |
| SHEET_DATA | Load all data of worksheet, such as cells data, settings, objects, ...etc. |
| BOOK_SETTINGS | Load settings for workbook |
| SETTINGS | Load settings for workbook and worksheet |
| XML_MAP | Load XmlMap |
| STRUCTURE | Load structure of the workbook |
| DOCUMENT_PROPERTIES | Load document properties |
| DEFINED_NAMES | Load defined Name objects |
| VBA | Load VBA projects |
| STYLE | Load styles for cell formatting |
| PICTURE | Load pictures |
| OLE_OBJECT | Load OleObjects |
| REVISION | Load revision logs |
### See Also
* module [`aspose.cells`](..)
