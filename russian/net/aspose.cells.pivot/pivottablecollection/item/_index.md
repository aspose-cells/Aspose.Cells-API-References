---
title: "PivotTableCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTableCollection. Получает отчёт PivotTable по индексу"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Получает отчёт PivotTable по индексу.

```csharp
public PivotTable this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте рабочую книгу из исходного файла
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к коллекции сводных таблиц
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Доступ к первой сводной таблице с помощью свойства Item (индексатор)
            PivotTable pivotTable = pivotTables[0];
            
            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();
            
            // Сохранить изменённую книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Получает отчёт PivotTable по имени PivotTable.

```csharp
public PivotTable this[string name] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать примерные данные
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Добавить сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Настроить сводную таблицу с помощью свойства Item
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Обновить и вычислить данные
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Доступ к сводной таблице с помощью свойства Item
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Изменить данные и обновить
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Сохраните книгу
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Получает [`PivotTable`](../../pivottable/) расположенный в ячейке.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Добавьте сводную таблицу на лист.
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Получить доступ к PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Продемонстрировать доступ к сводной таблице с использованием свойства Item (индексатор)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Продемонстрировать доступ по имени с использованием свойства Item
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // Настройте сводную таблицу
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Обновить и вычислить данные
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Сохраните книгу
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


