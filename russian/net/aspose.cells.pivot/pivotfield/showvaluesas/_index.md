---
title: "PivotField.ShowValuesAs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Показывает значения поля данных в разных форматах отображения, когда используется расчёт ShowDataAs"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/showvaluesas/
---
## ShowValuesAs(PivotFieldDataDisplayFormat, int, PivotItemPositionType, int) {#showvaluesas}

Показывает значения поля данных в разных форматах отображения, когда используется расчёт ShowDataAs.

```csharp
[Obsolete("Use PivotField.ShowValuesAs(PivotShowValuesAsType,int int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField, 
    PivotItemPositionType baseItemPositionType, int baseItem)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | Тип формата отображения данных. |
| baseField | Int32 | Индекс поля, на котором основан расчёт ShowDataAs. |
| baseItemPositionType | PivotItemPositionType | Тип позиции базового элемента. |
| baseItem | Int32 | Индекс базового элемента, на котором основан расчёт ShowDataAs. Работает только когда baseItemPositionType имеет значение custom. |

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте метод PivotField.ShowValuesAs(PivotShowValuesAsType,int,int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            worksheet.Name = "PivotData";

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Quarter");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue(1000);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue(1500);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Q1");
            worksheet.Cells["C4"].PutValue(800);
            
            worksheet.Cells["A5"].PutValue("Furniture");
            worksheet.Cells["B5"].PutValue("Q2");
            worksheet.Cells["C5"].PutValue(1200);

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Добавить поле строки
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields[rowFieldIndex];

            // Добавить поле столбца
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];

            // Добавить поле данных и настроить ShowValuesAs
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            dataField.DisplayName = "Sales Diff";
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);

            // Вычислите данные и сохраните
            pivotTable.CalculateData();
            workbook.Save("PivotTableShowValuesAsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, int, int) {#showvaluesas_1}

Устанавливает вычисление "Show Values As" для этого поля сводки.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, int baseField, int baseItem)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Тип расчёта "Show Values As". |
| baseField | Int32 | Индекс базового поля, используемого для расчёта. |
| baseItem | Int32 | Индекс базового элемента для расчёта. Используйте [`PreviousPivotItem`](../../pivotshowvaluessetting/previouspivotitem/) (-1) для предыдущего элемента, [`NextPivotItem`](../../pivotshowvaluessetting/nextpivotitem/) (-2) для следующего элемента; неотрицательные значения обозначают порядковый индекс конкретного элемента сводки. |

### Примечания

Только для поля данных.

### См. также

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## ShowValuesAs(PivotShowValuesAsType, string, string) {#showvaluesas_2}

Настраивает вычисление "Show Values As" для этого поля данных.

```csharp
public void ShowValuesAs(PivotShowValuesAsType showValuesAsType, string baseField, string baseItem)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| showValuesAsType | PivotShowValuesAsType | Тип расчёта для Show Values As. |
| baseField | String | Имя базового поля, используемого в расчёте. |
| baseItem | String | Подпись обычного элемента сводки. Также принимает зарезервированные литеральные ключевые слова: `(previous)` для предыдущего элемента, `(next)` для следующего элемента. Передайте `null`, если выбранный тип расчёта не требует базового элемента. |

### См. также

* enum [PivotShowValuesAsType](../../pivotshowvaluesastype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


