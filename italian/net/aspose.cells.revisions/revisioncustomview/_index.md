---
title: "Classe RevisionCustomView"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionCustomView. Rappresenta un record di revisione dell'aggiunta o rimozione di una vista personalizzata al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

Rappresenta un record di revisione dell'aggiunta o rimozione di una vista personalizzata alla cartella di lavoro

```csharp
public class RevisionCustomView : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | Ottiene il tipo di azione. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | Ottiene l'identificatore univoco globale della vista personalizzata. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | Ottiene il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCustomViewDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi una vista personalizzata per potenzialmente generare una revisione
                // Nota: utilizzo di CustomDocumentProperties come soluzione alternativa poiché CustomViews non è disponibile
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // Accedi ai log delle revisioni (supponendo che esistano)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Visualizza le proprietà di sola lettura
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // Dimostra l'uso base delle proprietà
                            if (customViewRevision.Type == RevisionType.CustomView)
                            {
                                Console.WriteLine("This is a custom view revision.");
                            }

                            if (customViewRevision.ActionType == RevisionActionType.Add)
                            {
                                Console.WriteLine("The custom view was added.");
                            }
                            else if (customViewRevision.ActionType == RevisionActionType.Delete)
                            {
                                Console.WriteLine("The custom view was deleted.");
                            }
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionCustomViewDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


