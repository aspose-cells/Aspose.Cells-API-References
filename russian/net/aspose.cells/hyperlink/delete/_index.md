---
title: "Hyperlink.Delete"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Hyperlink. Удаляет эту гиперссылку"
type: docs
url: /ru/net/aspose.cells/hyperlink/delete/
---
## Hyperlink.Delete method

Удаляет эту гиперссылку

```csharp
public void Delete()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkMethodDeleteDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько гиперссылок, чтобы продемонстрировать удаление
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
            
            Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
            
            // Удалить все гиперссылки
            for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
            {
                worksheet.Hyperlinks[i].Delete();
            }
            
            Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### См. также

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


