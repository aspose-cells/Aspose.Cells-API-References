---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Сохраняет все графические объекты как редактируемые формы в файле Word, чтобы вы могли редактировать их в Word"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Сохранить все графические объекты как редактируемые фигуры в файле Word, чтобы вы могли редактировать их в Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Примечания

Только для диаграмм.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // Инициализируйте DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Отобразить значение свойства SaveAsEditableShapes по умолчанию
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Установите SaveAsEditableShapes в true, чтобы продемонстрировать его использование
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Сохраните книгу в формате DOCX с настроенными параметрами
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


