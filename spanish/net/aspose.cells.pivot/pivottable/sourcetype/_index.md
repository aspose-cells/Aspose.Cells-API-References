---
title: "PivotTable.SourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene el tipo de fuente de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/sourcetype/
---
## PivotTable.SourceType property

Obtiene el tipo de origen de datos de la tabla dinámica.

```csharp
public PivotTableSourceType SourceType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertySourceTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Product A";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Product B";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Product C";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Muestra el valor actual de SourceType
            Console.WriteLine("Current PivotTable SourceType: " + pivotTable.SourceType);

            // Calcula los datos para mostrar la tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableSourceTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotTableSourceType](../../pivottablesourcetype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


