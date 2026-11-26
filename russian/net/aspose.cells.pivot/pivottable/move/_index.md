---
title: "PivotTable.Move"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Перемещает сводную таблицу в другое место листа"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/move/
---
## Move(int, int) {#move}

Перемещает сводную таблицу в другое место листа.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | индекс строки. |
| column | Int32 | индекс столбца. |

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotTable.MoveTo(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образцовые данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Вычислить данные для заполнения сводной таблицы
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table created at E3");

            try
            {
                // Переместить сводную таблицу в новое место (строка 10, столбец 5)
                pivotTable.Move(10, 5);
                Console.WriteLine("Pivot table moved to row 10, column 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("PivotTableMethodMoveWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(string) {#move_1}

Перемещает сводную таблицу в другое место листа.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(string destCellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| destCellName | String | имя целевой ячейки. |

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotTable.MoveTo(). Этот метод будет удалён через 12 месяцев, начиная с декабря 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Переместить сводную таблицу в новое место, используя имя ячейки
                pivotTable.Move("G10");

                Console.WriteLine("PivotTable moved successfully to G10");
                Console.WriteLine($"New location: {pivotTable.TableRange1.StartRow}, {pivotTable.TableRange1.StartColumn}");

                // Сохраните книгу
                workbook.Save("PivotTableMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error moving PivotTable: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


