---
title: "DataSorterKey.IconSetType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataSorterKey. Rappresenta il tipo di set di icone"
type: docs
url: /it/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Rappresenta il tipo di set di icone.

```csharp
public IconSetType IconSetType { get; }
```

### Osservazioni

Ha effetto solo quando [`Type`](../type/) è Icon.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con formattazione condizionale del set di icone
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

            // Crea un ordinatore di dati con tipo di set di icone
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Ordina i dati
            sorter.Sort(worksheet.Cells, area);

            // Mostra il tipo di set di icone dalla chiave dell'ordinatore
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Salva la cartella di lavoro
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


