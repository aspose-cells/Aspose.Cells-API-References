---
title: "Enum RevisionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionType enum. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

Rappresenta il tipo di revisione.

```csharp
public enum RevisionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| CustomView | `0` | Vista personalizzata. |
| DefinedName | `1` | Nome definito. |
| ChangeCells | `2` | Modifica delle celle. |
| AutoFormat | `3` | Formattazione automatica. |
| MergeConflict | `4` | Conflitto di unione. |
| Comment | `5` | Commento. |
| Format | `6` | Formato. |
| InsertSheet | `7` | Inserisci foglio di lavoro. |
| MoveCells | `8` | Sposta celle. |
| Undo | `9` | Annulla. |
| QueryTable | `10` | Interroga la tabella. |
| InsertDelete | `11` | Inserimento o eliminazione. |
| RenameSheet | `12` | Rinomina foglio di lavoro. |
| Unknown | `13` | Sconosciuto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Dimostrare l'uso di diversi valori enum RevisionType
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // Visualizzare i valori enum e i loro valori interi sottostanti
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // Dimostrare il controllo dei tipi di revisione
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


