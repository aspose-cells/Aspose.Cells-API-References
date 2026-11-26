---
title: "PageSetup.BlackAndWhite"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет, будут ли элементы документа печататься в чёрно‑белом виде"
type: docs
url: /ru/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Определяет, будут ли элементы документа печататься в чёрно‑белом виде.

```csharp
public bool BlackAndWhite { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить объект PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Установить свойство BlackAndWhite в true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Изменить свойство BlackAndWhite на false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Сохраните книгу
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


