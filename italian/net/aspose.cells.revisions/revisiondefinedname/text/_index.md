---
title: "RevisionDefinedName.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionDefinedName. Ottiene il testo del nome definito"
type: docs
url: /it/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Ottiene il testo del nome definito.

```csharp
public string Text { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un nome definito
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Modifica il nome definito per generare una revisione
            name.RefersTo = "=Sheet1!$B$1";
            
            // Salva su file per generare revisioni
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Riapri il file per leggere le revisioni
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Verifica le revisioni
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### Vedi anche

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


