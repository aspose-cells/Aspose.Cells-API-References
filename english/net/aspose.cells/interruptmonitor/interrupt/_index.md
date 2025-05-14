---
title: InterruptMonitor.Interrupt
second_title: Aspose.Cells for .NET API Reference
description: InterruptMonitor method. Interrupt the current operator
type: docs
url: /net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Interrupt the current operator.

```csharp
public void Interrupt()
```

### Examples

```csharp
// Called: monitor.Interrupt();
public void InterruptMonitor_Method_Interrupt()
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

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


