---
title: "RevisionHeader.UserName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionHeader. Ottiene e imposta il nome dell'utente che effettua la revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Ottiene e imposta il nome dell'utente che effettua la revisione.

```csharp
public string UserName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Crea un'istanza di RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Imposta la proprietà UserName
                revisionHeader.UserName = "JohnDoe";

                // Visualizza il valore corrente della proprietà UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Modifica la proprietà UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Salva la cartella di lavoro per dimostrare che la proprietà è in uso
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


