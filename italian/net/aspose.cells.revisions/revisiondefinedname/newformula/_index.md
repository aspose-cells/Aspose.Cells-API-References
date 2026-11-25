---
title: "RevisionDefinedName.NewFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionDefinedName. Ottiene la formula"
type: docs
url: /it/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Ottiene la formula.

```csharp
public string NewFormula { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e aggiungi alcuni dati
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // Aggiungi un nome definito che punta a A1
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifica il nome definito per generare una revisione (ora punta a B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Salva la cartella di lavoro per incorporare le informazioni di revisione
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Riapri la cartella di lavoro per leggere i log delle revisioni
                Workbook revWorkbook = new Workbook(fileName);

                // Itera attraverso le revisioni e visualizza NewFormula
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
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


