---
title: WorkbookDesigner.WorkbookDesigner
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner constructor. Initializes a new instance of the WorkbookDesigner class
type: docs
url: /net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner()
```

### Examples

```csharp
// Called: WorkbookDesigner designer = new WorkbookDesigner();
public void WorkbookDesigner_Constructor()
{
    List<Level> list = new List<Level>();
    for (int i = 1; i < 10001; i++)
    {
        list.Add(new Level("r" + i, "c" + i));
    }

    WorkbookDesigner designer = new WorkbookDesigner();
    designer.Workbook = PrepareCellsJava43994();

    ////currently it takes too long time to process normally
    //Console.WriteLine("CellsJava43994: Processing normally...");
    //DateTime t1 = DateTime.Now;
    //designer.SetDataSource("Level", list);
    //designer.CalculateFormula = false;
    //designer.Process();
    //int tt = (int)DateTime.Now.Subtract(t1).TotalMilliseconds;
    //Console.WriteLine("CellsJava43994: finished with time cost " + tt + "ms.");

    int tt = 15000; //large enough for assuring to interrupt after global processes has been finished
    designer.Workbook = PrepareCellsJava43994();
    Thread monitor = Util.StartInterruptMonitorThread(designer.Workbook,
        "CellsJava43994", tt / 5, tt / 10, true);
    designer.SetDataSource("Level", list);
    designer.CalculateFormula = false;
    designer.Process();
    monitor.Interrupt();
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |

### Examples

```csharp
// Called: WorkbookDesigner designer = new WorkbookDesigner(workbook);
public void WorkbookDesigner_Constructor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    String data = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}        }";

    WorkbookDesigner designer = new WorkbookDesigner(workbook);
    designer.SetJsonDataSource("ds", data);
    //designer.LineByLine = false;

    designer.Process();
    Assert.AreEqual("John Doe", workbook.Worksheets[0].Cells["A2"].StringValue);
}
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


