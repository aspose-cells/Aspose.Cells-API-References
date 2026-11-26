---
title: "Cell.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Verifica si este objeto se refiere a la misma celda que otro"
type: docs
url: /es/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Comprueba si este objeto se refiere a la misma celda que otro.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | otro objeto |

### Valor de retorno

true si dos objetos se refieren a la misma celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a celdas desde diferentes ubicaciones
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Establecer valores idénticos en diferentes celdas
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Comparar referencias de celda físicas idénticas
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Comparar diferentes celdas con contenido idéntico
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Comparar celda con un objeto que no sea una celda
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Comprueba si este objeto se refiere a la misma celda que otro objeto de celda.

```csharp
public bool Equals(Cell cell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| celda | Celda | otro objeto de celda |

### Valor de retorno

verdadero si dos objetos de celda se refieren a la misma celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear celdas en diferentes ubicaciones (A1 y B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Establecer valores idénticos en ambas celdas
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // Comparar cellA1 con cellB1 (diferentes ubicaciones)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // Comparar cellA1 consigo mismo (misma instancia)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


