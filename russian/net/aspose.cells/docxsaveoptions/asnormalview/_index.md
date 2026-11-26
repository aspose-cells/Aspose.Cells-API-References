---
title: "DocxSaveOptions.AsNormalView"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Экспорт Excel файла в docx как обычный вид. Если это свойство истинно, будет выведена одна область и масштаб не будет применяться. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Экспорт Excel‑файла в docx как обычный вид. Если это свойство истинно, будет выведена одна область, и масштаб не будет применяться. Значение по умолчанию — false.

```csharp
public bool AsNormalView { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Инициализируйте DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Отобразить значение свойства AsNormalView по умолчанию
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Установите AsNormalView в true, чтобы продемонстрировать его использование
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Сохраните книгу в формате DOCX с настроенными параметрами
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


