---
title: "PivotTableCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTableCollection. Удаляет PivotTable по указанному индексу и удаляет данные PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Удаляет PivotTable по указанному индексу и удаляет данные PivotTable

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс позиции в коллекции PivotTable |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Добавить несколько PivotTable
            sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");

            // Удалить сводную таблицу с индексом 1 (вторая сводная таблица)
            sheet.PivotTables.RemoveAt(1);

            // Проверьте количество после удаления
            Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Удаляет PivotTable по указанному индексу

```csharp
public void RemoveAt(int index, bool keepData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс позиции в коллекции PivotTable |
| keepData | Boolean | Нужно ли сохранять данные PivotTable |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Продемонстрировать RemoveAt с keepData=true
            worksheet.PivotTables.RemoveAt(0, true);
            Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);

            // Добавить другую сводную таблицу
            index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Продемонстрировать RemoveAt с keepData=false
            worksheet.PivotTables.RemoveAt(0, false);
            Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
        }
    }
}
```

### См. также

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


