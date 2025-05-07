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
            Workbook w = new Workbook(Constants.sourcePath + "CELLSNET51570.xlsx");
            List<Data51564> list = new List<Data51564>();
            Data51564 d = new Data51564();
            d.email = "asdf";
            d.employeeId = "123";
            d.transactions = new List<Transaction>();
            Transaction t = new Transaction();
            t.orderId = "10";
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
            des.SetDataSource("data", list);
            des.Process();
            Assert.AreEqual(75, w.Worksheets[0].Cells.GetRowHeightPixel(11));
            w.Save(Constants.destPath + "CELLSNET51570.xlsx");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


