---
title: "PivotTable.Fields"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Получает конкретные поля по типу поля"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Получает конкретные поля по типу поля.

```csharp
[Obsolete("Use PivotField.GetFields(PivotFieldType) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldType | PivotFieldType | тип поля. |

### Возвращаемое значение

конкретная коллекция полей

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод PivotField.GetFields(PivotFieldType). Этот метод будет удалён через 12 месяцев, начиная с мая 2024 года. Aspose просит прощения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "Sheet";

            // Пример данных
            ws.Cells[0, 0].PutValue("X");
            ws.Cells[0, 1].PutValue("Y");
            ws.Cells[0, 2].PutValue("Data");

            ws.Cells[1, 0].PutValue("A");
            ws.Cells[1, 1].PutValue("C");
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue("A");
            ws.Cells[2, 1].PutValue("D");
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue("B");
            ws.Cells[3, 1].PutValue("C");
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue("B");
            ws.Cells[4, 1].PutValue("D");
            ws.Cells[4, 2].PutValue(45);

            // Создать сводную таблицу
            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
            PivotTable pt = ptc[index];

            // Добавьте поля и продемонстрируйте метод Fields с PivotFieldType
            int fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
            PivotField rowField = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
            PivotField colField = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            PivotField dataField = pt.Fields(PivotFieldType.Data)[fp];

            // Добавьте второе поле данных с вычислением процента
            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            dataField = pt.Fields(PivotFieldType.Data)[fp];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            pt.RefreshData();
            pt.CalculateData();

            wb.Save("PivotTableFieldsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


