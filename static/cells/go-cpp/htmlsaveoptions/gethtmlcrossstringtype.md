##GetHtmlCrossStringType Method
'GetHtmlCrossStringType method. Encapsulates the function that represents gethtmlcrossstringtype in Go.'
## GetHtmlCrossStringType function
Indicates if a cross-cell string will be displayed in the same way as MS Excel when saving an Excel file in html format.By default the value is Default, so, for cross-cell strings, there is little difference between the html files created by Aspose.Cells and MS Excel.But the performance for creating large html files,setting the value to Cross would be several times faster than setting it to Default or Fit2Cell.
```go
func (instance *HtmlSaveOptions) GetHtmlCrossStringType()  (HtmlCrossType,  error)
```
## Remarks
## See Also
* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
