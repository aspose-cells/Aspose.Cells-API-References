---
title: "PageSetup.CenterHorizontally"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, печатается ли лист по горизонтали по центру"
type: docs
url: /ru/net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Определяет, печатается ли лист по‑горизонтали по центру.

```csharp
public bool CenterHorizontally { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }

            PageSetup pageSetup = worksheet.PageSetup;
            
            // Продемонстрировать свойство CenterHorizontally
            pageSetup.CenterHorizontally = true;
            pageSetup.PrintArea = "A1:B6";

            workbook.Save("CenterHorizontallyDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


