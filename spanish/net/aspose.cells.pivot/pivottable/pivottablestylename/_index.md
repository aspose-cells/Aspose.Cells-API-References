---
title: "PivotTable.PivotTableStyleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene o establece el nombre de estilo de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/pivottablestylename/
---
## PivotTable.PivotTableStyleName property

Obtiene o establece el nombre del estilo de la tabla dinámica.

```csharp
public string PivotTableStyleName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Data;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotTableStyleNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aplica un estilo de tabla dinámica incorporado
            pivotTable.PivotTableStyleName = "PivotStyleLight16";
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


