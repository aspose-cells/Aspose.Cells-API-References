---
title: "PivotTable.RemoveField"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Удаляет поле из определённой области"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Удаляет поле из конкретной области полей

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | Тип области полей. |
| fieldName | String | Имя в базовых полях. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Удалить поле "c" из области Data
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Вычислить данные сводной таблицы
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Удаляет поле из конкретного региона сводной таблицы.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | Тип области полей. |
| baseFieldIndex | Int32 | Индекс поля в базовых полях. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Удалить поле строки (индекс 0) из сводной таблицы
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Удалить поле из конкретной области полей

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | тип области полей. |
| pivotField | PivotField | поле в базовых полях. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Удалить поле столбца из сводной таблицы
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Удалить поле данных из сводной таблицы
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Сохраните книгу
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


