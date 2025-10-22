##MainWeb.IgnoreStyleWithNoData
MainWeb property. Gets or sets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true the performance will be better. The default value is false which means that if the last consecutive row/column has no cell values but is styled we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true which means GridWeb will show all rows/columns with style
## MainWeb.IgnoreStyleWithNoData property
Gets or sets whether GridWeb ignores showing rows or columns that do not contain cell values but are still styled. If set to true, the performance will be better. The default value is false, which means that if the last consecutive row/column has no cell values but is styled, we will still display them. This option is only valid when EnableAsync is false. This option has no effect when EnableAsync is true, which means GridWeb will show all rows/columns with style.
```csharp
public bool IgnoreStyleWithNoData { get; set; }
```
### See Also
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)
