##GetLegendEntries Method
'GetLegendEntries method. Encapsulates the function that represents getlegendentries in Go.'
## GetLegendEntries function
Gets a collection of all the LegendEntry objects in the specified chart legend.Setting the legend entries of the surface chart is not supported.So it will return null if the chart type is surface chart type.
```go
func (instance *Legend) GetLegendEntries()  (*LegendEntryCollection,  error)
```
## Remarks
## See Also
* Class [Legend](../)
* Library [Aspose.Cells for Go](../../)
