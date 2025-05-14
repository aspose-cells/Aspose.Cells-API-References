---
title: Workbook.InterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the interrupt monitor
type: docs
url: /net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Gets and sets the interrupt monitor.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Examples

```csharp
// Called: workbook.InterruptMonitor = monitor;
public void Workbook_Property_InterruptMonitor()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA42341_";

    DateTime start = DateTime.Now;
    Workbook workbook = new Workbook(filePath + "example.xlsx");

    InterruptMonitor monitor = new InterruptMonitor();
    workbook.InterruptMonitor = monitor;
    try
    {
        Console.WriteLine("Now convert");
        monitor.Interrupt();
        workbook.Save(CreateFolder(filePath) + "out.pdf", SaveFormat.Pdf);
        Console.WriteLine("Converted in " + DateTime.Now.Subtract(start).Milliseconds + "ms");
    }
    catch (CellsException e)
    {
        if (e.Code == ExceptionType.Interrupted)
        {
            Console.WriteLine("The save thread interrupted in " + DateTime.Now.Subtract(start).Milliseconds + "ms");
        }
        else
        {
            throw e;
        }
    }
}
```

### See Also

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


