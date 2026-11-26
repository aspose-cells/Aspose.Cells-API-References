---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает ширину столбца в разных представлениях"
type: docs
url: /ru/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Устанавливает ширину столбца в разных представлениях.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| column | Int32 | Индекс столбца. |
| пиксели | Int32 | Ширина в пикселях. |

### Примечания

Если текущий тип представления — PageLayoutView, ширина столбца совпадает с печатной шириной.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Установить примерные данные
            sheet.Cells[0, 0].Value = "Sample Text";

            // Вычислить ширину в пикселях (100 пикселей в этом примере)
            int pixelWidth = 100;

            // Установить ширину столбца в пикселях
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


