---
title: "Enumeración PivotTableAutoFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Pivot.PivotTableAutoFormatType. Representa el tipo de formato automático de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Representa el tipo de formato automático de la tabla dinámica.

```csharp
public enum PivotTableAutoFormatType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Representa el tipo de formato Ninguno. |
| Classic | `1` | Representa el tipo de formato automático Clásico. |
| Report1 | `2` | Representa el tipo de formato Report1. |
| Report2 | `3` | Representa el tipo de formato Report2. |
| Report3 | `4` | Representa el tipo de formato Report3. |
| Report4 | `5` | Representa el tipo de formato Report4. |
| Report5 | `6` | Representa el tipo de formato Report5. |
| Report6 | `7` | Representa el tipo de formato Report6. |
| Report7 | `8` | Representa el tipo de formato Report7. |
| Report8 | `9` | Representa el tipo de formato Report8. |
| Report9 | `10` | Representa el tipo de formato Report9. |
| Report10 | `11` | Representa el tipo de formato Report10. |
| Table1 | `12` | Representa el tipo de formato Table1. |
| Table2 | `13` | Representa el tipo de formato Table2. |
| Table3 | `14` | Representa el tipo de formato Table3. |
| Table4 | `15` | Representa el tipo de formato Table4. |
| Table5 | `16` | Representa el tipo de formato Table5. |
| Table6 | `17` | Representa el tipo de formato Table6. |
| Table7 | `18` | Representa el tipo de formato Table7. |
| Table8 | `19` | Representa el tipo de formato Table8. |
| Table9 | `20` | Representa el tipo de formato Table9. |
| Table10 | `21` | Representa el tipo de formato Table10. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de ejemplo para la tabla dinámica
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Agregar una PivotTable a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Establece el tipo de formato automático para la tabla dinámica
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Guarda el libro de trabajo
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


