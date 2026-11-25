---
title: "Cell.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell metodo. Verifica se questo oggetto si riferisce alla stessa cella di un altro"
type: docs
url: /it/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Verifica se questo oggetto si riferisce alla stessa cella di un altro.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | un altro oggetto |

### Valore di ritorno

vero se due oggetti si riferiscono alla stessa cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alle celle da posizioni diverse
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Imposta valori identici in celle diverse
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Confronta gli stessi riferimenti di cella fisici
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Confronta celle diverse con contenuto identico
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Confronta la cella con un oggetto non cella
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella.

```csharp
public bool Equals(Cell cell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cella | Cella | un altro oggetto cella |

### Valore di ritorno

vero se due oggetti cella si riferiscono alla stessa cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea celle in posizioni diverse (A1 e B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Imposta valori identici in entrambe le celle
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // Confronta cellA1 con cellB1 (posizioni diverse)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // Confronta cellA1 con se stessa (stessa istanza)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


