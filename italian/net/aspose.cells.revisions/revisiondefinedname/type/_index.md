---
title: "RevisionDefinedName.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionDefinedName. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Rappresenta il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea una nuova cartella di lavoro e aggiungi un nome definito
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modifica il nome definito per generare un record di revisione
                definedName.RefersTo = "=Sheet1!$B$1";

                // Salva la cartella di lavoro per incorporare le informazioni di revisione
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Riapri la cartella di lavoro per leggere il log delle revisioni
                Workbook revWb = new Workbook(filePath);

                // Itera attraverso le revisioni e visualizza il Tipo di ogni voce RevisionDefinedName
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


