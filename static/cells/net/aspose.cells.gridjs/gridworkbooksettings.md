##Class GridWorkbookSettings
Aspose.Cells.GridJs.GridWorkbookSettings class. Represents the settings of the workbook
## GridWorkbookSettings class
Represents the settings of the workbook.
```csharp
public class GridWorkbookSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Gets/sets the author of the file. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Indicates whether checking custom number format when setting Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Indicates whether create calculated formulas chain. Default is false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Indicates whether fully calculates every time when a calculation is triggered. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Indicates whether use iteration to resolve circular references. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Indicates whether re-calculate all formulas on opening file. Default is true. |
### Examples
```csharp
[C#]
GridJsWorkbook g = new GridJsWorkbook();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;
//do your business
[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()
Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
g.Settings=gsettings;
'do your business
```
### See Also
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)
