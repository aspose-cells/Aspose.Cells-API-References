---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает атрибут, который определяет записываемое имя ячейки (CellName). Например, если значение id, то для ячейки A1 вывод будет td idA1. Значение по умолчанию — null"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Указывает атрибут, в котором будет записано имя ячейки (CellName). (например, если значение \"id\", то для ячейки \"A1\" вывод будет: &lt;td id='A1'&gt;). Значение по умолчанию — null.

```csharp
public string CellNameAttribute { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Создайте примерную книгу с некоторыми данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Установите параметры сохранения HTML с CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // Сохраните в файл HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Проверьте, что вывод HTML содержит идентификаторы ячеек
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


