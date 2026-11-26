---
title: "PivotField.HideItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Устанавливает, скрыт ли конкретный PivotItem в поле данных."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Устанавливает, скрыт ли конкретный PivotItem в поле данных.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс pivotItem в pivotField. |
| isHidden | Boolean | скрыт ли конкретный PivotItem |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте свойство PivotField.PivotItems[int].IsHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу с примером сводной таблицы
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Пример данных для сводной таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Скрыть элементы, которые не являются "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Вычислить сводную таблицу
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Устанавливает, скрыт ли конкретный PivotItem в поле данных.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| itemValue | String | Имя pivotItem в pivotField. |
| isHidden | Boolean | Скрыт ли конкретный PivotItem |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте свойство PivotField.PivotItems[string].IsHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Вызовите метод HideItem с параметрами (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


