##Class GridWorkbookSettings
Aspose.Cells.GridWeb.Data.GridWorkbookSettings class. Represents settings of the workbook
## GridWorkbookSettings class
Represents settings of the workbook.
```csharp
public class GridWorkbookSettings : ISerializable
```
## Constructors
| Name | Description |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | default constructor |
## Properties
| Name | Description |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Gets and sets the author of the file. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Gets or sets whether checking custom number format when setting Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Gets or sets whether create calculated formulas chain. Default is false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Gets or sets the value which represents if the workbook uses the 1904 date system. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Gets or sets whether enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Gets or sets whether fully calculates every time when a calculation is triggered. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Gets or sets whether use iteration to resolve circular references. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Gets or sets the maximum number of iterations to resolve a circular reference,the default value is 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Gets or sets whether re-calculate all formulas on opening file. |
### Examples
```csharp
[C#]
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;
//do your business
[Visual Basic]
Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
gridweb.Settings=gsettings;
'do your business
```
### See Also
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)
