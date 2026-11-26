---
title: "PageSetup.FooterMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет расстояние от нижней части страницы до нижнего колонтитула в сантиметрах."
type: docs
url: /ru/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Представляет расстояние от нижнего края страницы до нижнего колонтитула, в сантиметрах.

```csharp
public double FooterMargin { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установите отступ нижнего колонтитула в сантиметрах
            pageSetup.FooterMargin = 1.5;

            // Добавьте немного содержимого, чтобы увидеть эффект
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Установите текст нижнего колонтитула, чтобы отступ был виден
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Сохраните книгу
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


