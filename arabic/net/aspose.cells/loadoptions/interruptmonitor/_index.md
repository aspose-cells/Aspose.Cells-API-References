---
title: "LoadOptions.InterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل وتعيّن مراقب المقاطعة"
type: docs
url: /ar/net/aspose.cells/loadoptions/interruptmonitor/
---
## LoadOptions.InterruptMonitor property

يحصل على ويضبط مراقب المقاطعة.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
            
            MemoryStream stream = new MemoryStream();
            workbook.Save(stream, SaveFormat.Xlsx);
            stream.Seek(0, SeekOrigin.Begin);

            Workbook loadedWorkbook = new Workbook(stream, new LoadOptions { 
                InterruptMonitor = new CustomInterruptMonitor() 
            });

            loadedWorkbook.Save("Output.xlsx");
        }
    }

    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested 
        { 
            get { return false; }
        }
    }
}
```

### انظر أيضًا

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


