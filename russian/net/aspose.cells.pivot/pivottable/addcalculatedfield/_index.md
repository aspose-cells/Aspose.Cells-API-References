---
title: "PivotTable.AddCalculatedField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Добавляет вычисляемое поле к полю сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Добавляет вычисляемое поле к полю сводной таблицы.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя вычисляемого поля |
| формула | String | Формула вычисляемого поля. |
| dragToDataArea | Boolean | True,перетащите это поле в область данных немедленно |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить вычисляемое поле
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // Сохраните книгу
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Добавляет вычисляемое поле к полю сводной таблицы и перетаскивает его в область данных.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя вычисляемого поля |
| формула | String | Формула вычисляемого поля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // Создать коллекцию сводных таблиц
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Добавить сводную таблицу и получить её индекс
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // Получить объект сводной таблицы
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Добавить поля в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Добавить вычисляемое поле
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // Форматировать поле данных
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


