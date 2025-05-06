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
[Test]
        public void Type_InterruptMonitor()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42341_&quot;;

            DateTime start = DateTime.Now;
            Workbook workbook = new Workbook(filePath + &quot;Mkw-50.xlsx&quot;);

            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            try
            {
                Console.WriteLine(&quot;Now convert&quot;);
                monitor.Interrupt();
                workbook.Save(CreateFolder(filePath) + &quot;out.pdf&quot;, SaveFormat.Pdf);
                Console.WriteLine(&quot;Converted in &quot; + DateTime.Now.Subtract(start).Milliseconds + &quot;ms&quot;);
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine(&quot;The save thread interrupted in &quot; + DateTime.Now.Subtract(start).Milliseconds + &quot;ms&quot;);
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


