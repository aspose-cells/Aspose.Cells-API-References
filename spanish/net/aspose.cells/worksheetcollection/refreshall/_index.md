---
title: "WorksheetCollection.RefreshAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Actualiza todas las tablas dinámicas y gráficos con la fuente dinámica"
type: docs
url: /es/net/aspose.cells/worksheetcollection/refreshall/
---
## WorksheetCollection.RefreshAll method

Actualiza todas las tablas dinámicas y gráficos con la fuente dinámica.

```csharp
[Obsolete("Use Workbook.RefreshAll() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RefreshAll()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Workbook.RefreshAll(). Este método será eliminado 12 meses después a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshAllDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y fórmulas
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Agregar fórmulas que serán actualizadas
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["C2"].PutValue("=SUM(B2:B3)");
            
            // Cambiar algunos valores
            worksheet.Cells["B2"].PutValue(3.0);
            worksheet.Cells["B3"].PutValue(2.0);
            
            // Actualizar todas las fórmulas en todas las hojas de cálculo
            workbook.Worksheets.RefreshAll();
            
            // Mostrar el total actualizado
            Console.WriteLine("Refreshed total: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


