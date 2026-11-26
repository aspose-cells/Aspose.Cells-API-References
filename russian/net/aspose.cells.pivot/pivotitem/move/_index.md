---
title: "PivotItem.Move"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotItem. Перемещает элемент вверх или вниз"
type: docs
url: /ru/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Перемещает элемент вверх или вниз

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| смещение | Int32 | Количество перемещений вверх или вниз. Переместить элемент вверх, если значение меньше нуля; переместить элемент вниз, если значение больше нуля. |
| isSameParent | Boolean | Указывает, происходит ли операция перемещения в том же родительском узле или нет |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotTable.MoveItem(PivotFieldType, string[],bool,int) или метод PivotItem.Move(int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать примерные данные для сводной таблицы
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Получите элементы сводной таблицы и продемонстрируйте метод Move
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Переместить первый элемент на позицию 1 (вторую позицию) вместе с дочерними элементами
            items[0].Move(1, true);
            
            // Сохраните книгу
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Перемещает элемент вверх или вниз в поле сводки

```csharp
public void Move(int offset)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| смещение | Int32 | Количество перемещений вверх или вниз. Переместить элемент вверх, если значение меньше нуля; переместить элемент вниз, если значение больше нуля. |

### См. также

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


