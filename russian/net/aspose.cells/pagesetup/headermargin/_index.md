---
title: "PageSetup.HeaderMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет расстояние от верхней части страницы до заголовка в единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Представляет расстояние от верхнего края страницы до верхнего колонтитула, в сантиметрах.

```csharp
public double HeaderMargin { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить поле заголовка в сантиметрах
            pageSetup.HeaderMargin = 1.5;

            // Проверить, что поле заголовка было установлено
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Сохраните книгу
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


