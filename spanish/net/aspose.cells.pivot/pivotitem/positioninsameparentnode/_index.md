---
title: "PivotItem.PositionInSameParentNode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Especifica el índice de posición en los PivotItems bajo el mismo nodo padre"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

Especificar el índice de posición en los PivotItems bajo el mismo nodo padre.

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int PositionInSameParentNode { get; set; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotTable.MoveItem(PivotFieldType, string[],bool,int). Este método será eliminado 12 meses después a partir de noviembre de 2026. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionInSameParentNodeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Agregar una nueva hoja de cálculo para la tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Agregar tabla dinámica
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configurar tabla dinámica
            PivotField vendorField = pivotTable.RowFields["Vendor"];
            vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demostrar la propiedad PositionInSameParentNode
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Establecer posiciones dentro del mismo nodo padre
            items["4H12"].PositionInSameParentNode = 1;
            items["DIF400"].PositionInSameParentNode = 2;
            
            // Recalcular después de cambiar posiciones
            pivotTable.CalculateData();
            
            // Establecer posiciones para otro grupo
            items["CA32"].PositionInSameParentNode = 1;
            items["AAA3"].PositionInSameParentNode = 2;

            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


