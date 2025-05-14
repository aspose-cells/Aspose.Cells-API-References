---
title: WorkbookDesigner.RepeatFormulasWithSubtotal
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether repeating formulas with subtotal row
type: docs
url: /net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Indicates whether repeating formulas with subtotal row.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Examples

```csharp
// Called: designer.RepeatFormulasWithSubtotal = true;
public void WorkbookDesigner_Property_RepeatFormulasWithSubtotal()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    DataTable dt = workbook.Worksheets[0].Cells.ExportDataTable(0, 0, 9, 7, true);
    dt.TableName = "products1";
    Workbook tem = new Workbook(Constants.sourcePath + "example.xlsx");
    WorkbookDesigner designer = new WorkbookDesigner(tem);
    designer.RepeatFormulasWithSubtotal = true;
    designer.SetDataSource(dt);
    designer.Process();
    Assert.AreEqual("=SUM(C5:D5)", tem.Worksheets[0].Cells["E5"].Formula);
    tem.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


