---
title: "RevisionQueryTable.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionQueryTable. Rappresenta il tipo della revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisionquerytable/type/
---
## RevisionQueryTable.Type property

Rappresenta il tipo della revisione.

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

    public class RevisionQueryTablePropertyTypeDemo
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
                // In uno scenario reale, otterresti le revisioni dal workbook
                // Per dimostrazione, creeremo un esempio concettuale
                // Nota: le istanze di RevisionQueryTable sono tipicamente ottenute dalle revisioni della cartella di lavoro

                // Crea una RevisionQueryTable simulata (questo è concettuale - in realtà la otterresti dalle revisioni)
                // Poiché non possiamo istanziare direttamente RevisionQueryTable, dimostreremo il modello
                RevisionQueryTable revisionQueryTable = null;

                // Verifica se abbiamo una tabella di query di revisione
                if (revisionQueryTable != null)
                {
                    // Visualizza il valore della proprietà Type (sola lettura)
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);

                    // Mostra il valore enum come intero per riferimento
                    Console.WriteLine("Revision Type (numeric): " + (int)revisionQueryTable.Type);

                    // Visualizza altre proprietà per contesto
                    Console.WriteLine("Cell Area: " + revisionQueryTable.CellArea);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample RevisionType values:");
                    Console.WriteLine("QueryTable = " + (int)RevisionType.QueryTable);
                    Console.WriteLine("ChangeCells = " + (int)RevisionType.ChangeCells);
                    Console.WriteLine("InsertSheet = " + (int)RevisionType.InsertSheet);
                }

                // Salva la cartella di lavoro
                workbook.Save("TypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


