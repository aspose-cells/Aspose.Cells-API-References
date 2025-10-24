##GridCell.Formula
GridCell property. Gets or sets a formula of the GridCell
## GridCell.Formula property
Gets or sets a formula of the [`GridCell`](../).
```csharp
public string Formula { get; set; }
```
### Remarks
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimeter, such as "=SUM(A1, E1, H2)".
User can set any formula in Workbook designer file. Aspose.Cells will keep all the formulas. If user use this property to set a formula to a cell, major part of Workbook built-in functions is supported. And more is coming. If you have any special need for Workbook built-in functions, please let us know.
### Examples
```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
ridWorksheet sheet = GridWeb1.ActiveSheet;
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1";
Visual Basic]
im GridWeb1 As GridWeb =  New GridWeb()
im sheet As GridWorksheet =  GridWeb1.ActiveSheet
heet.Cells["B6"].Formula = "=SUM(B2:B5, E1) + sheet1!A1"
```
### See Also
* class [GridCell](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
