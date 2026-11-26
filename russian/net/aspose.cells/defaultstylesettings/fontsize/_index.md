---
title: "DefaultStyleSettings.FontSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DefaultStyleSettings. Получает/задает стандартный размер шрифта по умолчанию для книги"
type: docs
url: /ru/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Получает/Устанавливает стандартный размер шрифта по умолчанию для книги.

```csharp
public double FontSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Задать имя шрифта и размер по умолчанию
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Загрузить HTML‑файл с этими настройками
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Получить доступ к ячейке и отобразить её размер шрифта
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### См. также

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


