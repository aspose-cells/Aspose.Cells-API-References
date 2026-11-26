---
title: "WriteProtection.RecommendReadOnly"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WriteProtection. Указывает, выбран ли параметр «Read Only Recommended»"
type: docs
url: /ru/net/aspose.cells/writeprotection/recommendreadonly/
---
## WriteProtection.RecommendReadOnly property

Указывает, выбран ли параметр «Рекомендуется только чтение».

```csharp
public bool RecommendReadOnly { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyRecommendReadOnlyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к рабочему листу и добавить примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Установите RecommendReadOnly в true
            workbook.Settings.WriteProtection.RecommendReadOnly = true;
            
            // Проверьте, что свойство установлено
            Console.WriteLine("RecommendReadOnly: " + workbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("IsWriteProtected: " + workbook.Settings.WriteProtection.IsWriteProtected);

            // Сохраните книгу
            workbook.Save("output_recommend_readonly.xlsx");

            // Загрузите сохранённую рабочую книгу, чтобы проверить, что настройки сохраняются
            Workbook loadedWorkbook = new Workbook("output_recommend_readonly.xlsx");
            Console.WriteLine("After loading - RecommendReadOnly: " + loadedWorkbook.Settings.WriteProtection.RecommendReadOnly);
            Console.WriteLine("After loading - IsWriteProtected: " + loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### См. также

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


