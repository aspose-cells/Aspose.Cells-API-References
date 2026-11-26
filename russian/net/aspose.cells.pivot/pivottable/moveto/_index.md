---
title: "PivotTable.MoveTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Перемещает сводную таблицу в другое место листа"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

Перемещает сводную таблицу в другое место листа.

```csharp
public void MoveTo(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | индекс строки. |
| column | Int32 | индекс столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            try
            {
                // Вызвать метод MoveTo с параметрами (Int32, Int32) для перемещения сводной таблицы
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // Пересчитать данные, чтобы обновить перемещённую сводную таблицу
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(int, int, int) {#moveto_1}

Перемещает сводную таблицу в другое место листа.

```csharp
public void MoveTo(int sheetIndex, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndex | Int32 | индекс целевого листа |
| строка | Int32 | индекс строки. |
| column | Int32 | индекс столбца. |

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_2}

Перемещает сводную таблицу в другое место листа.

```csharp
public void MoveTo(string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destCellName | String | имя целевой ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodMoveToWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить примерные данные
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Создать сводную таблицу
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            
            // Добавить поля в сводную таблицу
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Установить стиль и обновить
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            sheet.RefreshPivotTables();

            // Переместить сводную таблицу в новое место
            pivot.MoveTo("H16");
            sheet.RefreshPivotTables();

            // Сохраните книгу
            book.Save("PivotTableMoveToExample.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


