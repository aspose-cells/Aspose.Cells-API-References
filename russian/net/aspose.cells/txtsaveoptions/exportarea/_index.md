---
title: "TxtSaveOptions.ExportArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Диапазон ячеек для экспорта"
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

Диапазон ячеек для экспорта.

```csharp
public CellArea ExportArea { get; set; }
```

### Примечания

Если диапазон экспорта указан, [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) не будет иметь эффекта.

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить ячейки данными
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // Настройте параметры сохранения текста с ExportArea
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Сохранить только указанный диапазон (первые 3 строки, первые 2 столбца)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


