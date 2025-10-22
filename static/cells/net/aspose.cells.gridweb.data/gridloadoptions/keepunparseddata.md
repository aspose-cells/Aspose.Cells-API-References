##GridLoadOptions.KeepUnparsedData
GridLoadOptions property. Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true
## GridLoadOptions.KeepUnparsedData property
Whether keep the unparsed data in memory for the Workbook when it is loaded from template file. Default is true.
```csharp
public bool KeepUnparsedData { get; set; }
```
### Remarks
For scenarios that user only needs to read some contents from template file and does not need to save the workbook back, set this property as false may improve performance, especially when using it together with some kind of LoadFilter,
### See Also
* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
