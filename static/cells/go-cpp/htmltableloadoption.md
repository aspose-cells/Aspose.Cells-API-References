##HtmlTableLoadOption Class
'HtmlTableLoadOption class. Encapsulates the object that represents htmltableloadoption in Go.'
## HtmlTableLoadOption class
Represents the option when import table from html.
```go
type HtmlTableLoadOption struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewHtmlTableLoadOption](./newhtmltableloadoption/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetTableIndex](./gettableindex/) | Get or set the index of table to import from html. |
|[SetTableIndex](./settableindex/) | Get or set the index of table to import from html. |
|[GetId](./getid/) | Get or set the id of table to import from html |
|[SetId](./setid/) | Get or set the id of table to import from html |
|[GetOriginalSheetIndex](./getoriginalsheetindex/) | Get or set the original index of worksheet in the html. |
|[SetOriginalSheetIndex](./setoriginalsheetindex/) | Get or set the original index of worksheet in the html. |
|[GetTargetSheetIndex](./gettargetsheetindex/) | Get or set the target index of worksheet where the table is to be located. |
|[SetTargetSheetIndex](./settargetsheetindex/) | Get or set the target index of worksheet where the table is to be located. |
|[GetTableToListObject](./gettabletolistobject/) | Indicates whether generate list objects from imported table.The default value is false. |
|[SetTableToListObject](./settabletolistobject/) | Indicates whether generate list objects from imported table.The default value is false. |
