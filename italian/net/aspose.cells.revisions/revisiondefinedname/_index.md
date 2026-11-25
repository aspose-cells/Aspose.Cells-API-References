---
title: "Classe RevisionDefinedName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionDefinedName. Rappresenta un record di revisione di una modifica al nome definito"
type: docs
url: /it/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Rappresenta un record di revisione di una modifica di nome definito.

```csharp
public class RevisionDefinedName : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Ottiene la formula. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Ottiene la formula precedente. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Ottiene il testo del nome definito. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Rappresenta il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi un nome definito alla cartella di lavoro
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifica il nome definito per creare una revisione
                definedName.RefersTo = "=Sheet1!$B$1";

                // Salva la cartella di lavoro per generare i log delle revisioni
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Riapri la cartella di lavoro per accedere alle informazioni sulla revisione
                Workbook revisionWorkbook = new Workbook(filePath);

                // Itera i log delle revisioni per trovare le voci RevisionDefinedName
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Visualizza le proprietà di RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


