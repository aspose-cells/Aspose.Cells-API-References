---
title: "LoadOptions.InterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene y establece el monitor de interrupción"
type: docs
url: /es/net/aspose.cells/loadoptions/interruptmonitor/
---
## LoadOptions.InterruptMonitor property

Obtiene y establece el monitor de interrupción.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Ejemplos

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

### Ver también

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


