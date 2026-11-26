---
title: "StyleFlag.FontStrike"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка зачеркивания шрифта будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Настройка зачеркивания шрифта будет применена.

```csharp
public bool FontStrike { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Создайте объект стиля и установите FontStrike в true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Создайте флаг стиля и включите флаг FontStrike
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Примените стиль к ячейке с флагом стиля
            cell.SetStyle(style, styleFlag);

            // Отобразите текущий статус FontStrike
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Создайте другую ячейку, чтобы продемонстрировать текст без зачеркивания
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


