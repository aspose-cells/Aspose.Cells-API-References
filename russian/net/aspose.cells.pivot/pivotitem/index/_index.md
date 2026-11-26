---
title: "PivotItem.Index"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotItem. Возвращает индекс элемента сводки в поле кэша"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Возвращает индекс элемента сводки в поле кэша.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotItem.Position. Этот метод будет удалён через 6 месяцев, начиная с августа 2026 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Получить поле строки
            PivotField rowField = pivotTable.RowFields[0];
            
            // Получить доступ к элементам сводки с помощью свойства Index
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Скрыть детали элемента с помощью свойства Index
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Вычислить и обновить сводную таблицу
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Сохраните книгу
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


