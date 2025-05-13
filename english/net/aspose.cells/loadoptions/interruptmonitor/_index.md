---
title: LoadOptions.InterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and sets the interrupt monitor
type: docs
url: /net/aspose.cells/loadoptions/interruptmonitor/
---
## LoadOptions.InterruptMonitor property

Gets and sets the interrupt monitor.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Examples

```csharp
// Called: wb = new Workbook(ms, new LoadOptions() { InterruptMonitor = new CustomInterruptMonitor() });
public void LoadOptions_Property_InterruptMonitor()
{
    Workbook wb = new Workbook();
    Model.RandomFill(wb.Worksheets[0].Cells, 1000, 20, false);
    MemoryStream ms = Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
    ms.Seek(0, SeekOrigin.Begin);
    wb = new Workbook(ms, new LoadOptions() { InterruptMonitor = new CustomInterruptMonitor() });
    Util.ReSave(wb, SaveFormat.Xlsx);
}
```

### See Also

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


