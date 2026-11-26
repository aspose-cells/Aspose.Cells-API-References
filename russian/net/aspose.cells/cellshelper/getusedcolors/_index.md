---
title: "CellsHelper.GetUsedColors"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получает все используемые цвета в рабочей книге"
type: docs
url: /ru/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Получает все используемые цвета в рабочей книге.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| рабочая книга | Рабочая книга | Объект рабочей книги. |

### Возвращаемое значение

Используемые цвета.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько раскрашенных ячеек, чтобы продемонстрировать используемые цвета
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // Вызовите метод GetUsedColors с параметром workbook
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Отобразите используемые цвета
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


