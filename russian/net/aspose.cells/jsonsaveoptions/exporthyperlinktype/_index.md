---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonSaveOptions. Представляет тип экспорта гиперссылки в JSON"
type: docs
url: /ru/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

Представляет тип экспорта гиперссылок в JSON.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Примечания

Значение по умолчанию — DisplayString;

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте гиперссылку в ячейку A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Установите параметры экспорта для JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Сохранить книгу в JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Проверьте, что вывод содержит гиперссылку
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### См. также

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


