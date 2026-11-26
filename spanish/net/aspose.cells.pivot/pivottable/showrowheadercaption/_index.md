---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si el título del encabezado de fila se muestra en el informe de PivotTable. Indica si se muestran los títulos de los campos y los menús desplegables de filtro"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Indica si el título del encabezado de fila se muestra en el informe de PivotTable. Indica si se muestran los títulos de los campos y los menús desplegables de filtro

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.ShowHeaders. Este método será eliminado 12 meses después a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Agregar datos de muestra para la tabla dinámica
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Demostrar la propiedad ShowRowHeaderCaption
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


