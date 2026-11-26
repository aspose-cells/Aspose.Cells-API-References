---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontConfigs. Указывает, использовать ли системные заменители шрифтов в первую очередь, когда шрифт не представлен и заменитель этого шрифта не задан. Например, в Ubuntu шрифт Arial обычно заменяется на Liberation Sans. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Указывает, использовать ли сначала системные заменители шрифтов, когда шрифт не представлен и заменитель этого шрифта не установлен. Например, в Ubuntu шрифт \"Arial\" обычно заменяется на \"Liberation Sans\". Значение по умолчанию — false.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Отобразить текущее значение PreferSystemFontSubstitutes
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Установить PreferSystemFontSubstitutes в true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Создать ячейку со шрифтом, который может потребовать замену
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Сохранить рабочую книгу, чтобы увидеть эффекты замены шрифтов
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Сбросить к значению по умолчанию
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


