---
title: "PivotFilter.MeasureFldIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFilter. Возвращает индекс поля измерения фильтра сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Получает индекс поля измерения сводного фильтра.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте свойство PivotFilter.ValueFieldIndex. Этот метод будет удалён через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureFldIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 400;

            // Получить коллекцию сводных таблиц и добавить сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить коллекцию фильтров и добавить фильтр
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MeasureFldIndex = 1;

            workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


