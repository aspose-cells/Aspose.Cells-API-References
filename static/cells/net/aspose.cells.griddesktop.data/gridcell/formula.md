##GridCell.Formula
GridCell property. Gets or sets a formula of the Cell
## GridCell.Formula property
Gets or sets a formula of the Cell.
```csharp
public string Formula { get; set; }
```
### Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimeter, such as "=SUM(A1, E1, H2)".
User can set any formula in Workbook designer file. Aspose.Cells will keep all the formulas. If user use this property to set a formula to a cell, major part of Workbook built-in functions is supported. And more is coming. If you have any special need for Workbook built-in functions, please let us know.
### Examples
```csharp
[C#]
cell.Formula = "=SUM(A1:C3) + E6*2";
[Visual Basic]
cell.Formula = "=SUM(A1:C3) + E6*2"
```
### See Also
* class [GridCell](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
