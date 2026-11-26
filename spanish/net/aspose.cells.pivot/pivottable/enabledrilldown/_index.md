---
title: "PivotTable.EnableDrilldown"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si la profundización está habilitada"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Indica si la perforación está habilitada.

```csharp
public bool EnableDrilldown { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableDrilldownDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Configurar campos de la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Habilitar la funcionalidad de profundización
            pivotTable.EnableDrilldown = true;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
            
            // Verificar que la propiedad se haya establecido
            Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


