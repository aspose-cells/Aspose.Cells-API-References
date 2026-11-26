---
title: "Класс PivotFieldSortSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Pivot.PivotFieldSortSetting class. Представляет настройку сортировки полей сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldsortsetting/
---
## PivotFieldSortSetting class

Представляет настройку сортировки полей сводной таблицы.

```csharp
public class PivotFieldSortSetting
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Cell](../../aspose.cells.pivot/pivotfieldsortsetting/cell/) { get; } | Сортирует по значениям в строке или столбце. |
| [FieldIndex](../../aspose.cells.pivot/pivotfieldsortsetting/fieldindex/) { get; set; } | (**Obsolete.**) Представляет индекс поля, по которому производится сортировка. -1 означает сортировку PivotField по меткам, остальные значения означают сортировку по полю данных. |
| [IsSimpleSort](../../aspose.cells.pivot/pivotfieldsortsetting/issimplesort/) { get; set; } | Указывает, будет ли применена простая операция сортировки данных. |
| [IsSortByLabels](../../aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/) { get; } | Указывает, сортировать поле самостоятельно или по полю данных. |
| [LineTypeSortedBy](../../aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/) { get; } | Тип строки сводной таблицы, по которому выполнена сортировка. |
| [SortBy](../../aspose.cells.pivot/pivotfieldsortsetting/sortby/) { get; set; } | Представляет индекс поля, по которому выполнена сортировка. Значение -1 указывает на сортировку по собственным значениям элемента сводной таблицы. При значении, большем или равном нулю, представляет индекс поля данных в области данных. |
| [SortType](../../aspose.cells.pivot/pivotfieldsortsetting/sorttype/) { get; set; } | Представляет [`SortOrder`](../../aspose.cells/sortorder/). |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotFieldSortSettingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue("East");
            worksheet.Cells["B3"].PutValue("West");
            worksheet.Cells["B4"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Получить настройку сортировки поля сводной таблицы
            // Примечание: Предполагается, что у сводной таблицы есть настройки сортировки, к которым мы можем получить доступ.
            // Поскольку мы не можем создать новый PivotFieldSortSetting напрямую
            PivotFieldSortSetting sortSetting = pivotTable.RowFields[0].SortSetting;
            
            // Свойства отображения (только для чтения)
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("IsSortByLabels: " + sortSetting.IsSortByLabels);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("LineTypeSortedBy: " + sortSetting.LineTypeSortedBy);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);
            Console.WriteLine("Cell: " + sortSetting.Cell);

            // Применить сортировку к сводной таблице (фактическая сортировка будет выполнена через методы сводной таблицы)
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Сохранить результат
            workbook.Save("PivotFieldSortSettingDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


