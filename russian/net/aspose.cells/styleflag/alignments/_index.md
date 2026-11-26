---
title: "StyleFlag.Alignments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка выравнивания будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/alignments/
---
## StyleFlag.Alignments property

Настройка выравнивания будет применена.

```csharp
public bool Alignments { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyAlignmentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Создайте объект стиля и задайте свойства выравнивания
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.RotationAngle = 45;

            // Создайте флаг стиля и включите свойства выравнивания
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Alignments = true;

            // Примените стиль к ячейке с флагом стиля
            cell.SetStyle(style, styleFlag);

            // Отобразите текущие настройки выравнивания
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Измените флаг стиля, чтобы отключить свойства выравнивания
            styleFlag.Alignments = false;
            
            // Создайте новый стиль с другим выравниванием
            Style newStyle = workbook.CreateStyle();
            newStyle.HorizontalAlignment = TextAlignmentType.Right;
            newStyle.VerticalAlignment = TextAlignmentType.Top;
            newStyle.RotationAngle = 0;

            // Примените новый стиль — выравнивания не изменятся, потому что флаг установлен в false
            cell.SetStyle(newStyle, styleFlag);

            // Отобразите неизменённые настройки выравнивания
            Console.WriteLine("After applying new style with Alignments=false:");
            Console.WriteLine("Horizontal Alignment: " + cell.GetStyle().HorizontalAlignment);
            Console.WriteLine("Vertical Alignment: " + cell.GetStyle().VerticalAlignment);
            Console.WriteLine("Rotation: " + cell.GetStyle().RotationAngle);

            // Сохраните книгу
            workbook.Save("StyleFlagAlignmentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


