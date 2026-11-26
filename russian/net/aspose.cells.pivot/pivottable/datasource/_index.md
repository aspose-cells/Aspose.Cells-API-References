---
title: "PivotTable.DataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает и задает источник данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/datasource/
---
## PivotTable.DataSource property

Получает и задает источник данных сводной таблицы.

```csharp
public string[] DataSource { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataSourceDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Получить доступ и отобразить информацию об источнике данных
            string[] dataSource = pivotTable.DataSource;
            Console.WriteLine("Pivot Table Data Sources:");
            foreach (string source in dataSource)
            {
                Console.WriteLine(source);
            }
            
            // Сохраните книгу
            workbook.Save("PivotTableDataSourceDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


