---
title: WorkbookDesigner.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether formulas should be calculated
type: docs
url: /net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Indicates whether formulas should be calculated.

```csharp
public bool CalculateFormula { get; set; }
```

### Examples

```csharp
// Called: designer.CalculateFormula = true;
[Test]
        public void Property_CalculateFormula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SmartMarker/CellsNet42653.xlsx");
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Name";
            dr["Opportunity_Amount"] = "$1500.00";
            dt.Rows.Add(dr);
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true;
            designer.Process(false);
            Assert.AreEqual(workbook.Worksheets[0].Cells["C2"].Formula, "=CONCATENATE(K2,K3)");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


