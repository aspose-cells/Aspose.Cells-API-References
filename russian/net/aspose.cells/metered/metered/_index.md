---
title: "Metered.Metered"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор Metered. Инициализирует новый экземпляр этого класса"
type: docs
url: /ru/net/aspose.cells/metered/metered/
---
## Metered constructor

Инициализирует новый экземпляр этого класса.

```csharp
public Metered()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Создайте экземпляр, используя конструктор
            Metered metered = new Metered();

            // Установить лицензию Metered
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Создайте простой рабочий лист для демонстрации функциональности
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Сохраните книгу
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### См. также

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


