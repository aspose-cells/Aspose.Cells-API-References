---
title: "SaveOptions.ValidateMergedAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Указывает, следует ли проверять объединённые ячейки перед сохранением файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/validatemergedareas/
---
## SaveOptions.ValidateMergedAreas property

Указывает, следует ли проверять объединённые ячейки перед сохранением файла.

```csharp
public bool ValidateMergedAreas { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyValidateMergedAreasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить значения и объединить ячейки
            worksheet.Cells["A1"].PutValue("Merged Area");
            worksheet.Cells["A2"].PutValue("Test");
            worksheet.Cells.Merge(0, 0, 2, 1); // Merge A1:A2

            // Создать параметры сохранения с ValidateMergedAreas, установленным в true
            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ValidateMergedAreas = true,
                MergeAreas = true
            };

            // Сохранить книгу с проверкой объединённых областей
            workbook.Save("ValidateMergedAreasDemo.xlsb", saveOptions);

            Console.WriteLine("Workbook saved with merged areas validation.");
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


