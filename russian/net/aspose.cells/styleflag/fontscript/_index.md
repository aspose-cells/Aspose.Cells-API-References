---
title: "StyleFlag.FontScript"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка скрипта шрифта будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Настройка скрипта шрифта будет применена.

```csharp
public bool FontScript { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратитесь к ячейке A1 и задайте некоторый текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Создайте объект стиля и установите скрипт шрифта в нижний индекс
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Создайте флаг стиля и включите флаг FontScript
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Примените стиль к ячейке с флагом стиля
            cell.SetStyle(style, styleFlag);

            // Отобразите текущий статус скрипта шрифта
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Измените скрипт шрифта на верхний индекс
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Отобразите обновлённый статус скрипта шрифта
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Сохраните книгу
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


