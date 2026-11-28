---
title: "Workbook.InterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Kesinti izleyicisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Kesinti izleyicisini alır ve ayarlar.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına bazı veriler ekle
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Kesinti izleyicisini oluşturun ve atayın
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Uzun süren bir işlemi hemen keserek simüle et
                monitor.Interrupt();
                
                // Kaydetmeye çalış - kesintiye uğramalı
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine($"Error occurred: {e.Message}");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


