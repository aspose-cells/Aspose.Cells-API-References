---
title: "ExternalLinkCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExternalLinkCollection. Rimuove il collegamento esterno specificato dalla cartella di lavoro"
type: docs
url: /it/net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Rimuove il collegamento esterno specificato dalla cartella di lavoro.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice del collegamento esterno da rimuovere. |

### Osservazioni

Durante la rimozione del collegamento esterno, tutte le formule che vi fanno riferimento verranno rimosse perché i riferimenti diventano non validi.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con collegamenti esterni di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni collegamenti esterni di esempio
            worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
            worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
            worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";

            // Ottieni la collezione di collegamenti esterni
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Initial external links count: " + elc.Count);

            // Rimuovi i collegamenti esterni che non contengono "ImportantFiles" nel loro percorso
            for (int i = elc.Count - 1; i >= 0; i--)
            {
                if (!elc[i].DataSource.Contains("ImportantFiles"))
                {
                    elc.RemoveAt(i);
                }
            }

            Console.WriteLine("Remaining external links count: " + elc.Count);
            Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
        }
    }
}
```

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Rimuove il collegamento esterno specificato dalla cartella di lavoro.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice del collegamento esterno da rimuovere. |
| updateReferencesAsLocal | Boolean | Indica se aggiornare tutti i riferimenti del collegamento esterno fornito al riferimento della cartella di lavoro corrente. Controlla [`Clear`](../clear/) per ulteriori dettagli su questo parametro. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook wb = new Workbook();
            
            // Aggiungi alcuni collegamenti esterni
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
            elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
            elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
            elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });

            // Aggiungi alcune formule che fanno riferimento a questi collegamenti esterni
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
                }
            }

            Console.WriteLine($"Initial external links count: {elc.Count}");
            Console.WriteLine("Formulas before removal:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Rimuovi all'indice 1 con updateReferences=true
            elc.RemoveAt(1, true);
            
            Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Updated formulas:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Rimuovi all'indice 0 con updateReferences=false
            elc.RemoveAt(0, false);
            
            Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Formulas (should be cleared where references were removed):");
            for (int i = 0; i < 2; i++)
            {
                Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
            }
        }
    }
}
```

### Vedi anche

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


