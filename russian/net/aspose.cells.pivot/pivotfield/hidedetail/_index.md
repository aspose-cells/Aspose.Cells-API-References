---
title: "PivotField.HideDetail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Устанавливает, скрыты ли детали всех PivotItems в поле сводной таблицы. То есть сворачивает/разворачивает это поле"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Устанавливает, скрыты ли детали всех PivotItems в поле сводной таблицы. То есть сворачивает/разворачивает это поле.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isHiddenDetail | Boolean | Нужно ли скрывать детали поля сводной таблицы. |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте методы PivotItemsCollection.HideAllDetails() и UnhideAllDetails(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Компания Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Скрыть детали для первого поля строки
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


