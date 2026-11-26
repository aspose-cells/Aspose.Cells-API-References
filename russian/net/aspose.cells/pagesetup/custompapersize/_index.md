---
title: "PageSetup.CustomPaperSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает пользовательский размер листа в дюймах"
type: docs
url: /ru/net/aspose.cells/pagesetup/custompapersize/
---
## PageSetup.CustomPaperSize method

Устанавливает пользовательский размер бумаги в дюймах.

```csharp
public void CustomPaperSize(double width, double height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ширина | Double | Ширина листа. |
| высота | Double | Высота листа. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCustomPaperSizeWithDoubleDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить пользовательский размер листа (ширина: 1,5 дюйма, высота: 1,5 дюйма)
            worksheet.PageSetup.CustomPaperSize(1.5, 1.5);
            
            // Сохраните рабочую книгу, чтобы продемонстрировать эффект
            workbook.Save("CustomPaperSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


