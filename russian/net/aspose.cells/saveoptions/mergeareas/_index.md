---
title: "SaveOptions.MergeAreas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SaveOptions. Указывает, следует ли объединять области условного форматирования и проверки данных перед сохранением файла"
type: docs
url: /ru/net/aspose.cells/saveoptions/mergeareas/
---
## SaveOptions.MergeAreas property

Указывает, следует ли объединять области условного форматирования и проверки данных перед сохранением файла.

```csharp
public bool MergeAreas { get; set; }
```

### Примечания

Значение по умолчанию — false.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyMergeAreasDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните данные и создайте объединённые ячейки
            worksheet.Cells["A1"].PutValue("Merged Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Объедините ячейки A1:B1
            worksheet.Cells.Merge(0, 0, 1, 2);

            // Создайте параметры сохранения с включённым MergeAreas
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MergeAreas = true;

            // Сохраните с оптимизацией объединённых областей
            workbook.Save("MergeAreasDemo.xlsx", saveOptions);
        }
    }
}
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


