---
title: "Protection.AllowEditingScenario"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Представляет, разрешено ли пользователю редактировать сценарии на защищённом листе.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Получите доступ к настройкам защиты листа
            Protection protection = worksheet.Protection;

            // Установите свойства защиты с включённым AllowEditingScenario
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Защитить лист
            worksheet.Protect(ProtectionType.All);

            // Сохраните книгу
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


