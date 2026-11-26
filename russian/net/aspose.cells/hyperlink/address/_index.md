---
title: "Hyperlink.Address"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Hyperlink. Представляет адрес гиперссылки"
type: docs
url: /ru/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Представляет адрес гиперссылки.

```csharp
public string Address { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить гиперссылки с разными адресами
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Получить и отобразить адреса гиперссылок
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Сохраните книгу
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


