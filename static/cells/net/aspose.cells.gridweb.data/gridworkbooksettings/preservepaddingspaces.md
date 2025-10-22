##GridWorkbookSettings.PreservePaddingSpaces
GridWorkbookSettings property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
## GridWorkbookSettings.PreservePaddingSpaces property
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
```csharp
public bool PreservePaddingSpaces { get; set; }
```
### Remarks
Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.
### See Also
* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
