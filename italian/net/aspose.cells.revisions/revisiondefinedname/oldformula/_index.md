---
title: "RevisionDefinedName.OldFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionDefinedName. Ottiene la formula precedente"
type: docs
url: /it/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Ottiene la formula precedente.

```csharp
public string OldFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Aggiungi un nome definito per generare la cronologia delle revisioni
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifica il nome definito per creare una revisione
                definedName.RefersTo = "=Sheet1!$B$1";

                // Salva la cartella di lavoro per mantenere le revisioni
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Riapri la cartella di lavoro per accedere ai registri delle revisioni
                Workbook revisionWorkbook = new Workbook(filePath);

                // Itera attraverso i log delle revisioni per trovare le revisioni dei nomi definiti
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
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

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


