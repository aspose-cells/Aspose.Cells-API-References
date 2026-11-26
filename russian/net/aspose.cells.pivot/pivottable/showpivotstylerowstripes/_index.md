---
title: "PivotTable.ShowPivotStyleRowStripes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, применяется ли форматирование полос строк"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showpivotstylerowstripes/
---
## PivotTable.ShowPivotStyleRowStripes property

Указывает, применяется ли чередующееся форматирование строк.

```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleRowStripesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные
            DataTable data = new DataTable();
            data.Columns.Add("Category", typeof(string));
            data.Columns.Add("Product", typeof(string));
            data.Columns.Add("Sales", typeof(int));

            data.Rows.Add("Electronics", "Laptop", 1200);
            data.Rows.Add("Electronics", "Phone", 800);
            data.Rows.Add("Clothing", "Shirt", 50);
            data.Rows.Add("Clothing", "Pants", 70);
            data.Rows.Add("Furniture", "Chair", 150);
            data.Rows.Add("Furniture", "Table", 300);

            // Импортировать данные в лист
            worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить строки и столбцы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales

            // Включить полосы строк
            pivotTable.ShowPivotStyleRowStripes = true;

            // Вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохраните книгу
            workbook.Save("PivotTableWithRowStripes.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


