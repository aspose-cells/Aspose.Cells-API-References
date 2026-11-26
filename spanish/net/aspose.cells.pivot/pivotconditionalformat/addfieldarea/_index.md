---
title: "PivotConditionalFormat.AddFieldArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotConditionalFormat. Añade un área de campo de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Agrega un área del campo de tabla dinámica.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | PivotFieldType | El tipo de región. |
| fieldName | String | El nombre del campo dinámico. |

### Ejemplos

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
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
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

            // Crear tabla dinámica - corregido obteniendo la tabla dinámica del índice
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Agregar formato condicional
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Demostrar AddFieldArea con parámetros PivotFieldType y cadena
            pcf.AddFieldArea(PivotFieldType.Data, "Value");
            pcf.AddFieldArea(PivotFieldType.Row, "Category");

            // Agregar condición de formato
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();

            // Calcular datos y guardar
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Agrega un área del campo de tabla dinámica.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | PivotFieldType | El tipo de región. |
| campo | PivotField | El campo dinámico. |

### Ejemplos

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
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Agregue campos a áreas pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data

            // Agregar formato condicional
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            
            // Demostrar AddFieldArea con parámetros PivotFieldType y PivotField
            pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
            
            // Agregar condición de formato
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "100";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


