---
title: "DataSorterKey.IconId"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKey. Rappresenta l'ID del tipo di set di icone"
type: docs
url: /it/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Rappresenta l'ID del tipo di set di icone.

```csharp
public int IconId { get; }
```

### Osservazioni

Ha effetto solo quando [`Type`](../type/) è Icon.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con valori che potrebbero utilizzare set di icone
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi formattazione condizionale al set di icone
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Crea un ordinatore di dati e aggiungi la chiave
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Mostra la proprietà IconId dalle chiavi dell'ordinatore
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Salva la cartella di lavoro
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
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

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


