---
title: "StyleFlag.FontName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Будет применена настройка имени шрифта"
type: docs
url: /ru/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

Настройка названия шрифта будет применена.

```csharp
public bool FontName { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // Создать стили с разными именами шрифтов
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // Применить стиль заголовка с StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // Применить стиль цены с StyleFlag, сосредоточив внимание на FontName
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // Автоматически подгонять столбцы для лучшей видимости
            worksheet.AutoFitColumns();

            // Сохраните книгу
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


