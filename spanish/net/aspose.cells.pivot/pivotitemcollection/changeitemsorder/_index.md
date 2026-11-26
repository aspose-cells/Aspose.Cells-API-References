---
title: "PivotItemCollection.ChangeitemsOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotItemCollection. Cambia directamente el orden de los dos elementos"
type: docs
url: /es/net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Cambia directamente el orden de los dos elementos.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceIndex | Int32 | El índice actual |
| destIndex | Int32 | El índice de destino |

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método PivotItemCollection.SwapItem(). Este método será eliminado 12 meses después, a partir de julio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionMethodChangeitemsOrderWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[0, 0].Value = "Category";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[3, 0].Value = "C";

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:A4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            Console.WriteLine("Original Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            pivotItems.ChangeitemsOrder(0, 2);

            Console.WriteLine("\nAfter Changing Order:");
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(item.Name);
            }

            workbook.Save("PivotItemOrderChange.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


