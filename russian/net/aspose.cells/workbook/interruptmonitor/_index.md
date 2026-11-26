---
title: "Workbook.InterruptMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает и задает монитор прерываний"
type: docs
url: /ru/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Получает и задает монитор прерываний.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить некоторые данные в лист
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Создайте и назначьте монитор прерываний
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Смоделировать длительную операцию, прерывая её сразу
                monitor.Interrupt();
                
                // Попытка сохранить — должна быть прервана
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

### См. также

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


