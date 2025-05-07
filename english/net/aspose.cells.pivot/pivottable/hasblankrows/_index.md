---
title: PivotTable.HasBlankRows
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows
type: docs
url: /net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.

```csharp
public bool HasBlankRows { get; set; }
```

### Examples

```csharp
// Called: pt.HasBlankRows = false;
[Test]
        public void Property_HasBlankRows()
        {
            Workbook wb = new Workbook();
            wb.Worksheets.Add();

            Worksheet data = wb.Worksheets[0];
            int row = 0;

            data.Cells[row, 0].PutValue("Customer");
            data.Cells[row, 1].PutValue("Sku");
            data.Cells[row, 2].PutValue("Qty");
            Random r = new Random();
            for (row = 1; row < 50; row++)
            {
                data.Cells[row, 0].PutValue(r.Next(3) > 1 ? "Customer A" : "Customer B");
                data.Cells[row, 1].PutValue(r.Next(3) > 1 ? "Sku A" : "Sku B");
                data.Cells[row, 2].PutValue(r.Next(1, 100));
            }

            Worksheet pivot = wb.Worksheets[1];

            PivotTable pt = pivot.PivotTables[pivot.PivotTables.Add("=Sheet1!A1:C50", 0, 0, "Test pivot")];


            pt.EnableWizard = true;

            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.RowFields[0].IsAutoSubtotals = false;

            pt.AddFieldToArea(PivotFieldType.Row, 1);
            pt.RowFields[1].IsAutoSubtotals = false;

            pt.AddFieldToArea(PivotFieldType.Data, 2);

            pt.IsAutoFormat = true;
            pt.AutoFormatType = PivotTableAutoFormatType.Report5;
            pt.HasBlankRows = false;


            wb.Save(Constants.PivotTableDestPath + "Test_156592.xls");
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


