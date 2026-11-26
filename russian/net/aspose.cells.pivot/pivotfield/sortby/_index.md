---
title: "PivotField.SortBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Сортирует это поле сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Сортирует это сводное поле.

```csharp
public void SortBy(SortOrder sortType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | SortOrder | Тип сортировки этого поля. |

### См. также

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Сортирует это сводное поле.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | SortOrder | Тип сортировки этого поля. |
| fieldSortedBy | Int32 | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, другие значения означают индекс поля данных, по которому производится сортировка. |

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotField.SortBy(SortOrder, int,string) или свойство PivotField.IsAutoSort. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавить поле строки
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Отсортировать поле строки по убыванию с индексом -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Сортирует это сводное поле.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | SortOrder | Тип сортировки этого поля. |
| fieldSortedBy | Int32 | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, другие значения означают индекс поля данных, по которому производится сортировка. |
| dataType | PivotLineType | Тип данных, по которым производится сортировка. |
| cellName | String | Сортировать по значениям в строке или колонке |

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotField.SortBy(SortOrder, int,string). Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Добавить поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Отсортировать поле строки
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Вычислить данные
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Сортирует это сводное поле.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sortType | SortOrder | Тип сортировки этого поля. |
| fieldSortedBy | Int32 | Индекс поля сводной таблицы, по которому производится сортировка. -1 означает сортировку по меткам данных этого поля, другие значения означают индекс поля данных, по которому производится сортировка. |
| cellName | String | Сортировать по значениям в строке или колонке. Если Null, группировать по сумме поля, иначе группировать по значениям в выбранной колонке или строке. |

### См. также

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


