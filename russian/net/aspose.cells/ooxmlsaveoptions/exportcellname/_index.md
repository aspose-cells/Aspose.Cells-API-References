---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Указывает, следует ли экспортировать имена ячеек в файлы Excel2007 .xlsx .xlsm .xltx .xltm. Если выходной файл может быть доступен SQL Server DTS, это значение должно быть true. Установка значения в false значительно повысит производительность и уменьшит размер файла при создании больших файлов. Значение по умолчанию — true."
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Указывает, экспортировать ли имена ячеек в файл Excel2007 .xlsx (.xlsm, .xltx, .xltm). Если к выходному файлу может обращаться SQL Server DTS, это значение должно быть true. Установка значения в false значительно повысит производительность и уменьшит размер файла при создании больших файлов. Значение по умолчанию — true.

```csharp
public bool ExportCellName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Поместите некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Создайте параметры сохранения XLSX с включённым ExportCellName
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Сохраните книгу с экспортированными именами ячеек
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Создайте другие параметры сохранения с отключённым ExportCellName (по умолчанию)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Сохраните книгу без экспортированных имён ячеек
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### См. также

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


