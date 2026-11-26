---
title: "PageSetup.RightMargin"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PageSetup. Представляет размер правого поля в единицах сантиметров"
type: docs
url: /ru/net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Отображает размер правого поля в сантиметрах.

```csharp
public double RightMargin { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить разные правые поля и сохранить, чтобы продемонстрировать эффект
            worksheet.PageSetup.RightMargin = 0;
            workbook.Save("RightMargin_0.xlsx");

            worksheet.PageSetup.RightMargin = 1.0;
            workbook.Save("RightMargin_1.xlsx");

            worksheet.PageSetup.RightMargin = 2.5;
            workbook.Save("RightMargin_2.5.xlsx");

            // Вывести текущую величину правого поля
            Console.WriteLine("Current Right Margin: " + worksheet.PageSetup.RightMargin);
        }
    }
}
```

### См. также

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


