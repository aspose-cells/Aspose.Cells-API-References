---
title: "PivotFieldCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldCollection. Возвращает объект PivotField по указанному индексу"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Возвращает объект PivotField по указанному индексу.

```csharp
public PivotField this[int index] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист и получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Добавить сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Получите первое поле строки, используя свойство Item, и установите IsAutoSort
            pivotTable.RowFields[0].IsAutoSort = true;
            
            // Сохраните книгу
            workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Возвращает объект PivotField с указанным именем.

```csharp
public PivotField this[string name] { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "A";
            ws.Cells["B2"].Value = 10;
            ws.Cells["A3"].Value = "B";
            ws.Cells["B3"].Value = 20;
            ws.Cells["A4"].Value = "A";
            ws.Cells["B4"].Value = 30;
            ws.Cells["A5"].Value = "B";
            ws.Cells["B5"].Value = 40;

            // Создать сводную таблицу
            int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pTable = ws.PivotTables[index];
            
            // Добавить поля в сводную таблицу
            pTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Продемонстрировать использование свойства Item
            pTable.DataFields["Sum of Value"].IsAutoSort = true;
            pTable.DataFields["Sum of Value"].IsAscendSort = false;
            
            // Обновить и вычислить сводную таблицу
            pTable.RefreshData();
            pTable.CalculateData();
            
            // Сохраните книгу
            wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


