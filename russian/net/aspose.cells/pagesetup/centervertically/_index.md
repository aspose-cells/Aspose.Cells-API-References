---
title: "PageSetup.CenterVertically"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, печатается ли лист по вертикали по центру"
type: docs
url: /ru/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Определяет, печатается ли лист по‑вертикали по центру.

```csharp
public bool CenterVertically { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Обратиться к PageSetup и установить CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Добавьте некоторые примерные данные, чтобы визуализировать эффект
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Сохраните книгу
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


