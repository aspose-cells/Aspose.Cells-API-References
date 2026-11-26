---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Obtiene los nombres de las conexiones de datos de origen externas"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Obtiene los nombres de las conexiones de datos de origen externo.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // Crear tabla dinámica y obtener referencia
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Obtener conexiones de datos de origen
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // Mostrar la información de conexión
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


