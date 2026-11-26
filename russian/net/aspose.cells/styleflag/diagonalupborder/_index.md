---
title: "StyleFlag.DiagonalUpBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки диагональной верхней границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

Настройки диагональной верхней границы будут применены.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Создайте объект стиля и задайте диагональную верхнюю границу
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // Создайте флаг стиля и включите флаг диагональной верхней границы
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // Примените стиль с флагом к ячейке
            cell.SetStyle(style, styleFlag);

            // Создайте другую ячейку, чтобы продемонстрировать эффект
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // Создайте другой стиль для сравнения
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // Примените второй стиль с тем же флагом
            cell2.SetStyle(style2, styleFlag);

            // Сохраните книгу
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


