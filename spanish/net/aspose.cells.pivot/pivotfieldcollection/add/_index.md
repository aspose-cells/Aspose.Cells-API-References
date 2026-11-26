---
title: "PivotFieldCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotFieldCollection. Agrega un objeto PivotField al tipo específico PivotFields"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Agrega un objeto PivotField al tipo específico PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotField | PivotField | un objeto PivotField. |

### Valor de retorno

el índice del objeto PivotField en estos PivotFields.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la primera tabla dinámica
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            
            // Agregar campo de datos al área de campos de columna usando el método Add
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


