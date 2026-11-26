---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Указывает, экспортировать ли координаты Excel непустых ячеек при сохранении файла в html. Значение по умолчанию — false. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в ячейки
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Создать параметры сохранения HTML и включить ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Сохранить книгу в формате HTML с координатами ячеек
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


