---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel"
type: docs
url: /es/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Indica si se deben actualizar todas las conexiones al abrir el archivo en MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la colección de hojas de cálculo
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Agregar algunas hojas de cálculo de ejemplo
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Establecer la propiedad IsRefreshAllConnections
            worksheets.IsRefreshAllConnections = true;
            
            // Mostrar el valor actual de IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


