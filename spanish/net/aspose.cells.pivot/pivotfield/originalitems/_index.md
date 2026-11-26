---
title: "PivotField.OriginalItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtener los elementos base originales"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Obtenga los elementos base originales;

```csharp
public string[] OriginalItems { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyOriginalItemsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Acceder al primer campo de fila
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Mostrar elementos originales y elementos agrupados
            Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
            Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
            
            // Guardar el libro de trabajo modificado
            workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


