---
title: "SmartTagCollection.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagCollection. Ottiene la colonna dei smart tag della cella"
type: docs
url: /it/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

Ottiene la colonna dei tag intelligenti della cella.

```csharp
public int Column { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno smart tag alla cella C5 (riga 4, colonna 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // Ottieni la SmartTagCollection per la cella C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Visualizza la colonna della cella contenente questi smart tag
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // Aggiungi un altro smart tag alla cella E2 (riga 1, colonna 4) per dimostrare una colonna diversa
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


