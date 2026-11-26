---
title: "PivotItemCollection.SwapItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotItemCollection. Intercambia directamente dos elementos"
type: docs
url: /es/net/aspose.cells.pivot/pivotitemcollection/swapitem/
---
## PivotItemCollection.SwapItem method

Intercambia directamente dos elementos.

```csharp
public void SwapItem(int index1, int index2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| index1 | Int32 |  |
| index2 | Int32 |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemCollectionMethodSwapItemWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Obtener elementos de la tabla dinámica
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            try
            {
                // Mostrar orden original
                Console.WriteLine("Original order:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                // Intercambiar elementos en los índices 0 y 1
                pivotItems.SwapItem(0, 1);

                // Mostrar nuevo orden
                Console.WriteLine("\nAfter swapping:");
                foreach (PivotItem item in pivotItems)
                {
                    Console.WriteLine(item.Name);
                }

                Console.WriteLine("SwapItem method executed successfully with parameters (0, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SwapItem method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotItemCollectionMethodSwapItemWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


