---
title: "ImportTableOptions.DefaultValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImportTableOptions. Значение по умолчанию для ячейки в таблице — null"
type: docs
url: /ru/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

Значение по умолчанию для ячейки в таблице — null.

```csharp
public object[] DefaultValues { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пример данных с null‑значениями
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Отобразить начальное состояние
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Настройте значения по умолчанию для каждого столбца
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Импортировать данные с обработкой null
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Автоматически подгонять столбцы для лучшей видимости
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### См. также

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


