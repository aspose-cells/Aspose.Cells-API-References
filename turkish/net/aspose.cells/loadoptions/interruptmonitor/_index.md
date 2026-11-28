---
title: "LoadOptions.InterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Kesinti izleyicisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/interruptmonitor/
---
## LoadOptions.InterruptMonitor property

Kesinti izleyicisini alır ve ayarlar.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


