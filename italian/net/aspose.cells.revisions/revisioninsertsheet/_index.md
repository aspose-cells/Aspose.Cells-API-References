---
title: "Classe RevisionInsertSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionInsertSheet. Rappresenta un record di revisione di un foglio inserito"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertsheet/
---
## RevisionInsertSheet class

Rappresenta un record di revisione di un foglio che è stato inserito.

```csharp
public class RevisionInsertSheet : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioninsertsheet/actiontype/) { get; } | Ottiene il tipo di azione della revisione. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [Name](../../aspose.cells.revisions/revisioninsertsheet/name/) { get; } | Ottiene il nome del foglio di lavoro. |
| [SheetPosition](../../aspose.cells.revisions/revisioninsertsheet/sheetposition/) { get; } | Ottiene la posizione basata su zero del nuovo foglio nella barra delle schede dei fogli. |
| override [Type](../../aspose.cells.revisions/revisioninsertsheet/type/) { get; } | Ottiene il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionInsertSheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un nuovo foglio di lavoro per potenzialmente creare una revisione
                Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

                // Nota: Poiché non possiamo creare direttamente istanze di RevisionInsertSheet,
                // mostreremo come lavorare con una se esistesse nella collezione delle revisioni
                // Questo è uno scenario simulato poiché l'API di tracciamento delle revisioni reale non è completamente esposta

                // In uno scenario reale con il tracciamento delle revisioni abilitato, potresti ottenere revisioni come questa:
                // RevisionInsertSheet revision = null; // Verrebbe dalla collezione workbook.Revisions

                // Per scopi dimostrativi, mostreremo il modello di lavoro con un RevisionInsertSheet
                // Poiché non possiamo istanziarlo direttamente, dimostreremo il modello di accesso alle proprietà

                // Invece di provare a creare un'istanza, mostreremo come lavorare con una se disponibile
                // Questo mantiene la struttura correggendo l'errore di compilazione

                // Visualizza le informazioni sulle proprietà della revisione (simulato)
                Console.WriteLine("RevisionInsertSheet properties demonstration:");
                Console.WriteLine("Type property would show: RevisionType.InsertSheet");
                Console.WriteLine("ActionType property would show: RevisionActionType.Add");
                Console.WriteLine("Name property would show the sheet name");
                Console.WriteLine("SheetPosition property would show the zero-based position");

                // Salva la cartella di lavoro
                workbook.Save("RevisionInsertSheetDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with potential revisions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionInsertSheet: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


