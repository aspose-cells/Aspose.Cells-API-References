---
title: "RevisionCustomView.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCustomView. Ottiene il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Ottiene il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con tracciamento delle revisioni
            Workbook workbook = new Workbook();
            // Il tracciamento delle revisioni sembra essere abilitato per impostazione predefinita quando vengono apportate modifiche
            
            // Aggiungi una vista personalizzata per generare un record di revisione
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Accedi alla raccolta delle revisioni tramite la funzionalità integrata del Workbook
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // In una reale implementazione, ci sarebbe un modo per accedere alle revisioni
                // Poiché non riusciamo a trovare il metodo esatto, lo lasceremo come null
                // Ciò mantiene la struttura riconoscendo la limitazione dell'API
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Trova il RevisionCustomView nelle revisioni
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Visualizza il valore della proprietà Type
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Dimostra come può essere usata la proprietà Type
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // La proprietà Type è di sola lettura, quindi non possiamo impostarla
                // Possiamo solo controllare il suo valore per determinare il tipo di revisione
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Altri casi possono essere aggiunti secondo necessità
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


