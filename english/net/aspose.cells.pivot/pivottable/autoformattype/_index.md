---
title: PivotTable.AutoFormatType
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the auto format type of PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Gets and sets the auto format type of PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Examples

```csharp
// Called: pt.AutoFormatType = PivotTableAutoFormatType.Report5;
[Test]
        public void Property_AutoFormatType()
        {
            Workbook wb = new Workbook();
            wb.Worksheets.Add();

            Worksheet data = wb.Worksheets[0];
            int row = 0;

            data.Cells[row, 0].PutValue(&quot;Customer&quot;);
            data.Cells[row, 1].PutValue(&quot;Sku&quot;);
            data.Cells[row, 2].PutValue(&quot;Qty&quot;);
            Random r = new Random();
            for (row = 1; row &lt; 50; row++)
            {
                data.Cells[row, 0].PutValue(r.Next(3) &gt; 1 ? &quot;Customer A&quot; : &quot;Customer B&quot;);
                data.Cells[row, 1].PutValue(r.Next(3) &gt; 1 ? &quot;Sku A&quot; : &quot;Sku B&quot;);
                data.Cells[row, 2].PutValue(r.Next(1, 100));
            }

            Worksheet pivot = wb.Worksheets[1];

            PivotTable pt = pivot.PivotTables[pivot.PivotTables.Add(&quot;=Sheet1!A1:C50&quot;, 0, 0, &quot;Test pivot&quot;)];


            pt.EnableWizard = true;

            pt.AddFieldToArea(PivotFieldType.Row, 0);
            pt.RowFields[0].IsAutoSubtotals = false;

            pt.AddFieldToArea(PivotFieldType.Row, 1);
            pt.RowFields[1].IsAutoSubtotals = false;

            pt.AddFieldToArea(PivotFieldType.Data, 2);

            pt.IsAutoFormat = true;
            pt.AutoFormatType = PivotTableAutoFormatType.Report5;
            pt.HasBlankRows = false;


            wb.Save(Constants.PivotTableDestPath + &quot;Test_156592.xls&quot;);
        }
```

### See Also

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


