---
title: "Перечисление HtmlLayoutMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Rendering.HtmlLayoutMode. Представляет режим компоновки для HTML‑рендеринга"
type: docs
url: /ru/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Представляет режим компоновки для рендеринга HTML.

```csharp
public enum HtmlLayoutMode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Normal | `0` | Рендерит контент, как MS Excel. |
| Print | `1` | Рендерит контент в режиме печатной компоновки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить некоторые образцы данных в лист
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Создайте HtmlSaveOptions и установите режим компоновки в Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Сохраните книгу с обычным режимом компоновки
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Измените режим компоновки на Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Сохраните книгу с режимом печатной компоновки
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Отобразить значения перечисления
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


