---
title: "PivotField.HideItemDetail"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Устанавливает, скрыты ли детали конкретного PivotItem в поле сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Устанавливает, скрыты ли детали конкретного PivotItem в поле сводной таблицы.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс pivotItem в pivotField. |
| isHiddenDetail | Boolean | скрыт ли конкретный PivotItem |

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotField.PivotItems[int].IsDetailHidden. Этот метод будет удалён через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Добавьте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поля в области
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Получить поле сводной таблицы
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Скрыть детали элемента с индексом 2 (East), установив isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


