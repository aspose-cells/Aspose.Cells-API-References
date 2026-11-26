---
title: "PivotField.NonAutoSortDefault"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

Indica si una operación de ordenación que se aplicará a este pivot field es una operación de autoordenación o una ordenación de datos simple.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad !PivotField.SortSetting.IsSimpleSort. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Acceda a la primera hoja de cálculo y tabla dinámica
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Acceda al primer campo de fila en la tabla dinámica
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Establezca la propiedad NonAutoSortDefault en true
            pivotField.NonAutoSortDefault = true;
            
            // Mostrar el valor de la propiedad
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


