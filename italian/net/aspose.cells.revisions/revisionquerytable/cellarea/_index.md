---
title: "RevisionQueryTable.CellArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionQueryTable. Ottiene la posizione della tabella di query interessata"
type: docs
url: /it/net/aspose.cells.revisions/revisionquerytable/cellarea/
---
## RevisionQueryTable.CellArea property

Ottiene la posizione della tabella di query interessata.

```csharp
public CellArea CellArea { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionQueryTablePropertyCellAreaDemo
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
                RevisionQueryTable revisionQueryTable = null;

                // Verifica se abbiamo una tabella di query di revisione
                if (revisionQueryTable != null)
                {
                    // Visualizza il valore della proprietà CellArea (sola lettura)
                    Console.WriteLine("CellArea value: " + revisionQueryTable.CellArea);

                    // Visualizza altre proprietà per contesto
                    Console.WriteLine("Revision Type: " + revisionQueryTable.Type);
                    Console.WriteLine("Field ID: " + revisionQueryTable.FieldId);
                }
                else
                {
                    Console.WriteLine("No RevisionQueryTable available in this example.");
                    Console.WriteLine("In a real scenario, you would access this from workbook revisions.");
                    Console.WriteLine("Sample CellArea demonstration:");
                    Console.WriteLine("CellArea would represent the location of the query table, e.g., 'A1:B2'");
                }

                // Salva la cartella di lavoro
                workbook.Save("CellAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionQueryTable](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


