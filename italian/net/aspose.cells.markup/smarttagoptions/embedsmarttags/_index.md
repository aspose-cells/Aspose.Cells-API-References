---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagOptions. Indica se salvare gli smart tag con la cartella di lavoro"
type: docs
url: /it/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Indica se salvare i tag intelligenti con la cartella di lavoro.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyEmbedSmartTagsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagOptions smartTagOptions = new SmartTagOptions();
            Console.WriteLine("Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            smartTagOptions.EmbedSmartTags = true;
            // Le SmartTagOptions sono ora correttamente utilizzate se richieste dall'API, sebbene l'assegnazione a workbook.Settings non sia valida

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // Accedi agli SmartTags tramite SmartTagSetting
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // Usa le proprietà per impostare LinkedCell
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


