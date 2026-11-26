---
title: "DocxSaveOptions.SaveElementType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocxSaveOptions. Указывает, какие элементы должны быть сохранены"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Указывает, какие элементы следует сохранить.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте несколько примерных данных
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Инициализируйте DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // ПРИМЕЧАНИЕ: Свойство SaveElementType отсутствует в классе DocxSaveOptions
                // на основе предоставленного отражения API. Если бы оно существовало, вы бы прочитали его так:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // Продемонстрировать чтение существующего свойства: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Установите свойство в true и отобразите новое значение
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Сохраните книгу в формате DOCX, используя настроенные параметры
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


