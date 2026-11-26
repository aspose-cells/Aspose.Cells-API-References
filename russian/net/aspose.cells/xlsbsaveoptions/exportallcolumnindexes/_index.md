---
title: "XlsbSaveOptions.ExportAllColumnIndexes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsbSaveOptions. Указывает, экспортировать ли все индексы столбцов для ячеек"
type: docs
url: /ru/net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

Указывает, экспортировать ли все индексы столбцов для ячеек.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyExportAllColumnIndexesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["C2"].PutValue(3);

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ExportAllColumnIndexes = true // Demonstrate the property usage
            };

            workbook.Save("XlsbExportAllColumnIndexes.xlsb", saveOptions);
        }
    }
}
```

### См. также

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


