---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "HtmlSaveOptions property. Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — Normal"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Получает или задает режим компоновки при сохранении в HTML. Значение по умолчанию — Normal.

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Создать экземпляр HtmlSaveOptions
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Отобразите текущее значение LayoutMode
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Установите LayoutMode в Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Сохраните рабочую книгу с режимом компоновки Print
                workbook.Save("LayoutModePrint.html", options);

                // Установите LayoutMode в Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Сохраните рабочую книгу с режимом компоновки Normal
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


