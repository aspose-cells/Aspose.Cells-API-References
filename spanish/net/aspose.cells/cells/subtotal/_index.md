---
title: "Cells.Subtotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Crea subtotales para el rango"
type: docs
url: /es/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Crea subtotales para el rango.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango |
| groupBy | Int32 | El campo por el cual agrupar, como un desplazamiento entero basado en cero |
| función | ConsolidationFunction | La función de subtotal. |
| totalList | Int32[] | Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Puebla datos de muestra para subtotales
            CreateSampleData(worksheet);

            // Define el área de celdas que contiene los datos (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Llama al método Subtotal con los parámetros:
                // - Agrupar por la columna 0 (Región)
                // - Usar la función SUM
                // - Aplicar a la columna 2 (Ventas)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Los métodos ExpandColumnLevel y ExpandRowLevel fueron eliminados para corregir errores de compilación
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Crear fila de encabezado
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Crear filas de datos
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Poblar datos comenzando desde la fila 2 (índice base cero 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Crea subtotales para el rango.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango |
| groupBy | Int32 | El campo por el cual agrupar, como un desplazamiento entero basado en cero |
| función | ConsolidationFunction | La función de subtotal. |
| totalList | Int32[] | Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales. |
| reemplazar | Booleano | Indica si se reemplazan los subtotales actuales |
| pageBreaks | Booleano | Indica si se agrega un salto de página entre grupos |
| summaryBelowData | Booleano | Indica si se agrega un resumen debajo de los datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear datos de muestra para subtotales
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Definir el área de celdas para el subtotal (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Llamar a Subtotal con parámetros:
                // - Agrupar por la primera columna (índice base cero 0)
                // - Usar la función Sum
                // - Aplicar a la tercera columna (índice base cero 2)
                // - Reemplazar subtotales existentes, saltos de página entre grupos, resumen debajo de los datos
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


