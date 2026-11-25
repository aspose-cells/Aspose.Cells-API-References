---
title: "RevisionInsertSheet.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertSheet. Ottiene il nome del foglio di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

Ottiene il nome del foglio di lavoro.

```csharp
public string Name { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro per potenzialmente generare un record di revisione
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // Simula l'accesso a un RevisionInsertSheet dalle revisioni
                // Nota: In uno scenario reale, questo proviene da workbook.Revisions
                // Per dimostrazione, creeremo uno scenario simulato
                RevisionInsertSheet insertSheetRevision = null;

                // Nell'uso reale, otterresti questo dalla collezione delle revisioni
                // Ad esempio: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // Poiché non possiamo creare RevisionInsertSheet direttamente, dimostreremo
                // ciò che faresti se avessi accesso a uno
                if (insertSheetRevision != null)
                {
                    // Visualizza il valore della proprietà Name (sola lettura)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // Dimostra l'uso della proprietà Name in un controllo condizionale
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


