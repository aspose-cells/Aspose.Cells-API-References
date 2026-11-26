---
title: "PivotTable.EnableWizard"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si el asistente de tabla dinámica está disponible"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

Indica si el asistente de PivotTable está disponible.

```csharp
public bool EnableWizard { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableWizardDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 2000;

            // Agregar tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Desactivar el asistente de tabla dinámica
            pivotTable.EnableWizard = false;

            // Guarda el libro de trabajo
            workbook.Save("PivotTable_EnableWizard_Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


