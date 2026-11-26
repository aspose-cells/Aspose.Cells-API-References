---
title: "StyleFlag.FontUnderline"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Будет применена настройка подчеркивания шрифта"
type: docs
url: /ru/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Настройка подчеркивания шрифта будет применена.

```csharp
public bool FontUnderline { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Создать объект стиля и установить подчеркивание шрифта
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Создайте флаг стиля и включите флаг подчеркивания шрифта
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Примените стиль к ячейке с флагом стиля
            cell.SetStyle(style, styleFlag);

            // Отобразите текущий статус подчеркивания
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Измените тип подчеркивания на двойной
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Сохраните книгу
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


