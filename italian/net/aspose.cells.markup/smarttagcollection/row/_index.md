---
title: "SmartTagCollection.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagCollection. Ottiene la riga dei smart tag della cella"
type: docs
url: /it/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Ottiene la riga dei tag intelligenti della cella.

```csharp
public int Row { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un tag intelligente alla cella A1 (riga 0, colonna 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Ottieni la SmartTagCollection per la cella A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Visualizza la riga della cella contenente questi smart tag
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Nota: la proprietà Row è di sola lettura, quindi non possiamo impostarla
            // smartTags.Row = 5; // Questo causerebbe un errore di compilazione

            // Aggiungi un altro smart tag alla cella B3 (riga 2, colonna 1) per dimostrare una riga diversa
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


