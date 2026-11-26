---
title: "PivotConditionalFormat.AddFieldArea"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotConditionalFormat. Добавляет область поля сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Добавляет область поля сводной таблицы.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | PivotFieldType | Тип региона. |
| fieldName | String | Имя поля сводной таблицы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Создайте сводную таблицу — исправлено получением сводной таблицы по индексу
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Добавить условный формат
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Продемонстрируйте AddFieldArea с параметрами PivotFieldType и строкой
            pcf.AddFieldArea(PivotFieldType.Data, "Value");
            pcf.AddFieldArea(PivotFieldType.Row, "Category");

            // Добавить условие форматирования
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();

            // Вычислите данные и сохраните
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Добавляет область поля сводной таблицы.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| axisType | PivotFieldType | Тип региона. |
| поле | PivotField | Поле сводной таблицы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;

            // Создать сводную таблицу
            int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Добавить поля в области сводной таблицы
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data

            // Добавить условный формат
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            
            // Продемонстрируйте AddFieldArea с параметрами PivotFieldType и PivotField
            pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
            
            // Добавить условие форматирования
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "100";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.Red;

            // Сохраните книгу
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### См. также

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


