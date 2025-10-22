##SetExcludeUnusedStyles Method
'SetExcludeUnusedStyles method. Encapsulates the function that represents setexcludeunusedstyles in Go.'
## SetExcludeUnusedStyles function
Indicating whether excludes unused styles.For the generated html files, excluding unused styles can make the file size smallerwithout affecting the visual effects. So the default value of this property is true.If user needs to keep all styles in the workbook for the generated html(such as the scenario that userneeds to restore the workbook from the generated html later), please set this property as false.
```go
func (instance *HtmlSaveOptions) SetExcludeUnusedStyles(value bool)  error
```
## Remarks
## See Also
* Class [HtmlSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
