##WorkbookRender.CustomPrint
WorkbookRender method. Client can control page setting of printer when print each page using this function
## WorkbookRender.CustomPrint method
Client can control page setting of printer when print each page using this function.
```csharp
public int CustomPrint(bool nextPageAfterPrint, PrintPageEventArgs printPageEventArgs)
```
| Parameter | Type | Description |
| --- | --- | --- |
| nextPageAfterPrint | Boolean | If true , printer will go to next page after print current page |
| printPageEventArgs | PrintPageEventArgs | System.Drawing.Printing.PrintPageEventArgs |
### Return Value
Indirect next page index, based on zero
### See Also
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
