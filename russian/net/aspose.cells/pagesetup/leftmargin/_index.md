---
title: "PageSetup.LeftMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер левого поля в единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Представляет размер левого поля, в сантиметрах.

```csharp
public double LeftMargin { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Установите некоторые примерные данные
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Установить левое поле (в дюймах)
            sheet.PageSetup.LeftMargin = 1.5;

            // Выведите значение левого поля в консоль
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Сохраните в PDF, чтобы продемонстрировать поле
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


