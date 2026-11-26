---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldSortSetting. Указывает, следует ли сортировать поле по самому себе или по полю данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

Указывает, сортировать поле самостоятельно или по полю данных.

```csharp
public bool IsSortByLabels { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Получить настройку сортировки сводного поля
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Отобразить текущее значение IsSortByLabels
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // Примечание: IsSortByLabels только для чтения, поэтому мы не можем установить его напрямую
            // Вместо этого мы продемонстрируем его значение, изучив настройки сортировки

            // Показать связанные свойства сортировки
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // Сохраните книгу
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


