---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotFieldSortSetting. Указывает, будет ли применена простая сортировка данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Указывает, будет ли применена простая операция сортировки данных.

```csharp
public bool IsSimpleSort { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
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
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Создайте сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить сводное поле
            PivotField pivotField = pivotTable.RowFields[0];

            // Получить настройку сортировки (только для чтения)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Отобразить текущее значение IsSimpleSort
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Примечание: IsSimpleSort только для чтения, поэтому мы не можем установить его напрямую
            // Чтобы продемонстрировать сортировку, мы создадим новую сводную таблицу с другим порядком сортировки

            // Создать другую сводную таблицу с пользовательской сортировкой
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Отсортировать поле сводной таблицы с помощью доступного метода
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Сохраните книгу
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


