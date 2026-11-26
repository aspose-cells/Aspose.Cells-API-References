---
title: "PivotAreaCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotAreaCollection. Eliminar una configuración de área condicional formateada de tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotareacollection/removeat/
---
## PivotAreaCollection.RemoveAt method

Eliminar una configuración de área condicional formateada de tabla dinámica.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Definir áreas de celda para agregar a las áreas de tabla dinámica
            CellArea cellArea1 = new CellArea();
            cellArea1.StartRow = 0;
            cellArea1.StartColumn = 0;
            cellArea1.EndRow = 2;
            cellArea1.EndColumn = 1;

            CellArea cellArea2 = new CellArea();
            cellArea2.StartRow = 1;
            cellArea2.StartColumn = 1;
            cellArea2.EndRow = 3;
            cellArea2.EndColumn = 2;

            // Obtener la colección de áreas de tabla dinámica seleccionando el área
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
            pivotAreas.Add(cellArea2);

            try
            {
                // Mostrar las áreas de tabla dinámica antes de la eliminación
                Console.WriteLine("Pivot areas before removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }

                // Llame al método RemoveAt con el parámetro Int32
                pivotAreas.RemoveAt(0);

                Console.WriteLine("\nPivot areas after removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


