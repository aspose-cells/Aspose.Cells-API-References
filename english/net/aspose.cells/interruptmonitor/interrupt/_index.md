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
[Test]
        public void Method_Interrupt()
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

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


