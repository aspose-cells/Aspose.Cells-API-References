---
title: "StyleFlag.DiagonalDownBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки диагональной нижней границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/diagonaldownborder/
---
## StyleFlag.DiagonalDownBorder property

Настройки диагональной нижней границы будут применены.

```csharp
public bool DiagonalDownBorder { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalDownBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Diagonal Down Border Demo");

            // Создайте объект стиля и задайте диагональную нижнюю границу
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
            
            // Создайте флаг стиля и включите флаг диагональной нижней границы
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalDownBorder = true;

            // Примените стиль с флагом к ячейке
            cell.SetStyle(style, styleFlag);

            // Проверьте, включен ли флаг диагональной нижней границы
            Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Отключите флаг диагональной нижней границы
            styleFlag.DiagonalDownBorder = false;
            style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);

            // Примените стиль с флагом к ячейке
            cell.SetStyle(style, styleFlag);
            Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);

            // Сохраните книгу
            workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


