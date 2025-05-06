---
title: PivotShowValuesSetting.CalculationType
second_title: Aspose.Cells for .NET API Reference
description: PivotShowValuesSetting property. Represents how to show values of a data field in the pivot report
type: docs
url: /net/aspose.cells.pivot/pivotshowvaluessetting/calculationtype/
---
## PivotShowValuesSetting.CalculationType property

Represents how to show values of a data field in the pivot report.

```csharp
public PivotFieldDataDisplayFormat CalculationType { get; set; }
```

### Examples

```csharp
// Called: pf.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;
[Test]
        public void Property_CalculationType()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET42427_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(FileFormatType.Pdf);
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = &quot;Sheet&quot;;

            ws.Cells[0, 0].PutValue(&quot;X&quot;);
            ws.Cells[0, 1].PutValue(&quot;Y&quot;);
            ws.Cells[0, 2].PutValue(&quot;Data&quot;);

            ws.Cells[1, 0].PutValue(&quot;A&quot;);
            ws.Cells[1, 1].PutValue(&quot;C&quot;);
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue(&quot;A&quot;);
            ws.Cells[2, 1].PutValue(&quot;D&quot;);
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue(&quot;B&quot;);
            ws.Cells[3, 1].PutValue(&quot;C&quot;);
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue(&quot;B&quot;);
            ws.Cells[4, 1].PutValue(&quot;D&quot;);
            ws.Cells[4, 2].PutValue(45);

            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add(&quot;=Sheet!A1:C5&quot;, &quot;A7&quot;, &quot;PivotTable1&quot;);
            PivotTable pt = ptc[index];

            int fp; PivotField pf;

            fp = pt.AddFieldToArea(PivotFieldType.Row, &quot;X&quot;);
            pf = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, &quot;Y&quot;);
            pf = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, &quot;Data&quot;);
            pf = pt.Fields(PivotFieldType.Data)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, &quot;Data&quot;);
            pf = pt.Fields(PivotFieldType.Data)[fp];
            pf.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            wb.Save(savePath + &quot;out.xlsx&quot;);
            wb.Save(savePath + &quot;out.pdf&quot;);
            pt.RefreshData();
            pt.CalculateData();

            Assert.AreEqual(ws.Cells[&quot;C10&quot;].StringValue, &quot;25.00%&quot;);
            Assert.AreEqual(ws.Cells[&quot;E10&quot;].StringValue, &quot;35.71%&quot;);
            Assert.AreEqual(ws.Cells[&quot;G10&quot;].StringValue, &quot;31.82%&quot;);
           
        }
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


