---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Получает или задает значение, указывающее, следует ли преобразовывать строковое значение в числовое или дату"
type: docs
url: /ru/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Получает или задаёт значение, указывающее, следует ли преобразовывать строковое значение в числовое или дату.

```csharp
public bool ConvertNumericData { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создайте примерную таблицу данных с числовыми и строковыми значениями
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Получите ячейки первого рабочего листа
            Cells cells = workbook.Worksheets[0].Cells;

            // Создайте параметры импорта с ConvertNumericData, установленным в true
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Импортировать данные с числовым преобразованием
            cells.ImportData(dt, 0, 0, options);

            // Отобразить результаты
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


