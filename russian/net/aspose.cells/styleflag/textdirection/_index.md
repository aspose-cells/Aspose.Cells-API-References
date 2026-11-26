---
title: "StyleFlag.TextDirection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка направления текста будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

Настройка направления текста будет применена.

```csharp
public bool TextDirection { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // Создайте стиль и задайте направление текста
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // Создайте флаг стиля и включите флаг TextDirection
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // Примените стиль к ячейке с флагом стиля
            cell.SetStyle(style, styleFlag);

            // Отобразите текущее направление текста
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Измените направление текста и примените снова
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // Сохраните книгу
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


