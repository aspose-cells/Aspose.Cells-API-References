---
title: "Workbook.IsLicensed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Указывает, установлена ли лицензия"
type: docs
url: /ru/net/aspose.cells/workbook/islicensed/
---
## Workbook.IsLicensed property

Указывает, установлен ли лицензионный ключ.

```csharp
public bool IsLicensed { get; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsLicensedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Задайте несколько базовых свойств, чтобы продемонстрировать использование Workbook
            wb.Worksheets[0].Name = "Sheet1";
            wb.Worksheets[0].Cells[0, 0].PutValue("Sample Data");
            
            // Проверить, лицензирована ли книга
            Console.WriteLine($"IsLicensed: {wb.IsLicensed}");
            
            // Продемонстрировать различное поведение в зависимости от статуса лицензии
            if (wb.IsLicensed)
            {
                Console.WriteLine("Running in licensed mode - full features available");
            }
            else
            {
                Console.WriteLine("Running in evaluation mode - watermarks will appear");
            }

            // Сохранить в поток памяти для демонстрации функциональности
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                Console.WriteLine($"Workbook saved successfully (Size: {ms.Length} bytes)");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


