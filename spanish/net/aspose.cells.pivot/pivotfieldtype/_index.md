---
title: "Enum PivotFieldType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Pivot.PivotFieldType. Representa el tipo de campo de PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldtype/
---
## PivotFieldType enumeration

Representa el tipo de campo de tabla dinámica.

```csharp
public enum PivotFieldType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `0` | Presenta el tipo de campo base de pivote. |
| Row | `1` | Presenta el tipo de campo de fila de pivote. |
| Column | `2` | Presenta el tipo de campo de columna de pivote. |
| Page | `4` | Presenta el tipo de campo de página de pivote. |
| Data | `8` | Presenta el tipo de campo de datos de pivote. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldTypeDemo
    {
        public static void PivotFieldTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Agregar una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Establecer estilo de tabla pivot
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


