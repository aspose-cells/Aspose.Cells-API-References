---
title: WorkbookDesigner.LineByLine
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether processing the smart marker line by line
type: docs
url: /net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

Indicates whether processing the smart marker line by line.

```csharp
public bool LineByLine { get; set; }
```

### Remarks

The default value is true. If False, the template file must contain a range which is named as "_CellsSmartMarkers".

### Examples

```csharp
// Called: des.LineByLine = false;
[Test]
        public void Property_LineByLine()
        {
            Workbook w = new Workbook(Constants.sourcePath + &quot;CELLSNET51570.xlsx&quot;);
            List&lt;Data51564&gt; list = new List&lt;Data51564&gt;();
            Data51564 d = new Data51564();
            d.email = &quot;asdf&quot;;
            d.employeeId = &quot;123&quot;;
            d.transactions = new List&lt;Transaction&gt;();
            Transaction t = new Transaction();
            t.orderId = &quot;10&quot;;
            d.transactions.Add(t);
            d.transactions.Add(t);
            d.transactions.Add(t);
            d.transactions.Add(t);
            list.Add(d);
            list.Add(d);
            list.Add(d);
            list.Add(d);
            WorkbookDesigner des = new WorkbookDesigner(w);
            des.LineByLine = false;
            des.SetDataSource(&quot;data&quot;, list);
            des.Process();
            Assert.AreEqual(75, w.Worksheets[0].Cells.GetRowHeightPixel(11));
            w.Save(Constants.destPath + &quot;CELLSNET51570.xlsx&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


