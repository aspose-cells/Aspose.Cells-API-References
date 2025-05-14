---
title: Class InterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.InterruptMonitor class. Represents all operator about the interrupt
type: docs
url: /net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Represents all operator about the interrupt.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Constructors

| Name | Description |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Mark the monitor as requesting interruption |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) is true, a [`CellsException`](../cellsexception/) with code Interrupted will be thrown.(Inherited from [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Methods

| Name | Description |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Interrupt the current operator. |

### Examples

```csharp
// Called: InterruptMonitor monitor = new InterruptMonitor();
public void Cells_Type_InterruptMonitor()
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

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


