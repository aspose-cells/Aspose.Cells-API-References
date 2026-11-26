---
title: "Protection.AllowInsertingHyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешена ли вставка гиперссылок на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Представляет, разрешено ли вставка гиперссылок на защищённом листе

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // Добавьте гиперссылку, чтобы продемонстрировать функциональность
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


