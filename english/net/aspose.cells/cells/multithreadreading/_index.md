---
title: Cells.MultiThreadReading
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets whether the cells data model should support MultiThread reading. Default value of this property is false
type: docs
url: /net/aspose.cells/cells/multithreadreading/
---
## Cells.MultiThreadReading property

Gets or sets whether the cells data model should support Multi-Thread reading. Default value of this property is false.

```csharp
public bool MultiThreadReading { get; set; }
```

### Remarks

If there are multiple threads to read Row/Cell objects in this collection concurrently, this property should be set as true, otherwise unexpected result may be produced. Supporting Multi-Thread reading may degrade the performance for accessing Row/Cell objects from this collection. Please note, some features cannot support Multi-Thread reading, such as formatting values(by [`StringValue`](../../cell/stringvalue/), [`DisplayStringValue`](../../cell/displaystringvalue/), .etc.). So, even with this property being set as true, those APIs still may give unexpected result for Multi-Thread reading.

### Examples

```csharp
// Called: cells.MultiThreadReading = true;
public void Cells_Property_MultiThreadReading()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells.MultiThreadReading = true;
    Style style = wb.CreateStyle();
    style.Custom = "yyyy-mm-dd";
    StyleFlag sf = new StyleFlag();
    sf.All = true;
    cells.Columns[0].ApplyStyle(style, sf);
    int tc = 500;
    int tcc = 50;
    for (int i = tc * tcc - 1; i > -1; i--)
    {
        cells[i, 0].PutValue(44438 + i);
    }
    StringBuilder err = new StringBuilder();
    int[] finished = new int[] { 0 };
    for (int i = 0; i < tc; i++)
    {
        Thread t = new Thread(MultiFormat);
        t.Start(new object[] { cells, tcc * i, tcc * i + tcc, err, finished, });
    }
    tcc = 0;
    while (finished[0] < tc)
    {
        Thread.Sleep(500);
        tcc++;
        if (tcc > 20)
        {
            if (err.Length > 0)
            {
                Console.WriteLine("Errors:\n" + err.ToString(1, err.Length - 1));
            }
            Assert.Fail("Too long time to wait for all threads to finish. Currently finished: " + finished[0]);
            break;
        }
    }
    Console.WriteLine("Finished threads: " + finished[0]);
    if (err.Length > 0)
    {
        Assert.Fail(err.ToString(1, err.Length - 1));
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


