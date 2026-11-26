---
title: "PageSetup.IsHFAlignMargins"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Указывает, выравниваются ли поля заголовка и нижнего колонтитула с полями страницы. Если это свойство истинно, левый заголовок и нижний колонтитул будут выравнены с левым полем, а правый заголовок и нижний колонтитул — с правым полем. Эта опция включена по умолчанию"
type: docs
url: /ru/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Указывает, выравниваются ли поля верхнего и нижнего колонтитулов с полями страницы. Если это свойство истинно, левый верхний и нижний колонтитулы будут выравнены с левым полем, а правый верхний и нижний колонтитулы — с правым полем. Эта опция включена по умолчанию.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить IsHFAlignMargins в true
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Изменить IsHFAlignMargins на false
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Сохраните книгу
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


