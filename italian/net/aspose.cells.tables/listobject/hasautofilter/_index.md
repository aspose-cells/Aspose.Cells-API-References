---
title: "ListObject.HasAutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListObject. Indica se il filtro automatico è applicato a questa tabella"
type: docs
url: /it/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Indica se il filtro automatico è applicato a questa tabella.

```csharp
public bool HasAutoFilter { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Aggiungi un ListObject (tabella) che copre l'intervallo di dati
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Assicurati che la tabella sia ridimensionata per includere tutte le righe
                listObject.Resize(0, 0, 4, 2, true);

                // Leggi e visualizza il valore della proprietà HasAutoFilter
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // L'oggetto AutoFilter può essere accesso tramite la proprietà AutoFilter
                // Dimostra che non è nullo quando HasAutoFilter è vero
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Applica un filtro semplice sulla colonna "Score" (indice 1) per mostrare le righe con Score >= 80
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Usa Cells.Rows per verificare se la riga è nascosta
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Cancella il filtro
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


