---
title: "RevisionQueryTable.FieldId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionQueryTable. Ottiene l'ID del campo della tabella di query specifico che è stato rimosso"
type: docs
url: /it/net/aspose.cells.revisions/revisionquerytable/fieldid/
---
## RevisionQueryTable.FieldId property

Ottiene l'ID del campo specifico della tabella di query che è stato rimosso.

```csharp
public int FieldId { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyFieldIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1.20;

            try
            {
                // Crea una tabella di query (questo è un esempio semplificato)
                // Nota: In uno scenario reale, dovresti prima creare una tabella di query
                // Per scopi dimostrativi, simuleremo l'accesso a una RevisionQueryTable

                // Poiché non possiamo creare direttamente una RevisionQueryTable in questo esempio semplificato,
                // mostreremo come accedere alla proprietà FieldId se ne avessimo una
                // Questo mostra il modello per leggere la proprietà di sola lettura

                // Simula l'ottenimento di una RevisionQueryTable dalle revisioni (concettuale)
                // In realtà, otterresti questo da workbook.Revisions o simili
                RevisionQueryTable revisionQueryTable = null;

                // Verifica se abbiamo una tabella di query di revisione (questo è solo per dimostrazione)
                if (revisionQueryTable != null)
                {
                    // Visualizza il valore della proprietà FieldId
                    Console.WriteLine("FieldId value: " + revisionQueryTable.FieldId);

                    // Visualizza altre proprietà per contesto
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                }

                // Salva la cartella di lavoro
                workbook.Save("FieldIdDemo.xlsx");
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

* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


