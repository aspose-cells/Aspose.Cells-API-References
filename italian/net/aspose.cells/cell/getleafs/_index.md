---
title: "Cell.GetLeafs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottieni tutte le celle che fanno riferimento a questa cella direttamente e devono essere aggiornate quando questa cella viene modificata"
type: docs
url: /it/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Ottieni tutte le celle che fanno riferimento a questa cella direttamente e devono essere aggiornate quando questa cella viene modificata.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Valore di ritorno

Enumeratore per enumerare tutti i dipendenti (Cell)

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati e formule per creare dipendenze
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Ottieni la cella che ha dipendenti
                Cell cell = worksheet.Cells["B1"];

                // Chiama GetLeafs per ottenere tutte le celle che fanno riferimento a questa cella direttamente
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Ottieni tutte le celle che saranno aggiornate quando questa cella viene modificata.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ricorsivo | Booleano | Restituisce i leafs che non fanno riferimento a questa cella direttamente ma fanno riferimento ad altri leafs di questa cella |

### Valore di ritorno

Enumeratore per enumerare tutti i dipendenti (Cell)

### Osservazioni

NOTA: Questa classe è ora obsoleta. Invece, si prega di utilizzare Cell.GetDependentsInCalculation(bool) per ottenere tutti i dipendenti nella catena di calcolo. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati con formule per creare dipendenze
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Ottieni la cella che ha dipendenti
                Cell cell = worksheet.Cells["A1"];

                // Chiama GetLeafs con il parametro ricorsivo impostato su true
                IEnumerator leafs = cell.GetLeafs(true);

                // Visualizza i risultati
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Salva la cartella di lavoro
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


