---
title: "RevisionCustomView.ActionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCustomView. Ottiene il tipo di azione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Ottiene il tipo di azione.

```csharp
public RevisionActionType ActionType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Carica una cartella di lavoro esistente che potrebbe contenere revisioni di vista personalizzata
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Itera attraverso tutti i registri di revisione nella cartella di lavoro
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Controlla ogni revisione nel registro
                    foreach (Revision revision in log.Revisions)
                    {
                        // Verifica se questa è una revisione di vista personalizzata
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Visualizza il valore della proprietà ActionType
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Dimostra come utilizzare la proprietà ActionType
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Visualizza proprietà aggiuntive per il contesto
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


