---
title: "Range.Hyperlinks"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Возвращает все гиперссылки в диапазоне"
type: docs
url: /ru/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Получает все гиперссылки в диапазоне.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте гиперссылку в ячейку A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Создайте диапазон, содержащий A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Получите гиперссылки в диапазоне
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Отобразите информацию о гиперссылке
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Удалить гиперссылку
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Проверьте, что гиперссылка была удалена
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### См. также

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


