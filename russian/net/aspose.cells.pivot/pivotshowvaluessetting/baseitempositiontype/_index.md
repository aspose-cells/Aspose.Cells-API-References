---
title: "PivotShowValuesSetting.BaseItemPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotShowValuesSetting. Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. Поскольку PivotItemPosition.Custom только для чтения, если вам необходимо установить PivotItemPosition.Custom, пожалуйста, задайте атрибут PivotField.BaseItemIndex."
type: docs
url: /ru/net/aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/
---
## PivotShowValuesSetting.BaseItemPositionType property

Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. Поскольку PivotItemPosition.Custom только для чтения, если вам необходимо установить PivotItemPosition.Custom, пожалуйста, задайте атрибут PivotField.BaseItemIndex.

```csharp
[Obsolete("Use PivotShowValuesSetting.BaseItem property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotItemPositionType BaseItemPositionType { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotShowValuesSetting.BaseItem. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotShowValuesSettingPropertyBaseItemPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField dataField = pivotTable.DataFields[0];
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0;
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1;

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            workbook.Save("PivotShowValuesSettingExample.xlsx");
        }
    }
}
```

### См. также

* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotShowValuesSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


