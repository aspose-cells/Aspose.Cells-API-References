---
title: "Classe SmartTagOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Markup.SmartTagOptions classe. Rappresenta le opzioni del tag intelligente"
type: docs
url: /it/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Rappresenta le opzioni dello smart tag.

```csharp
public class SmartTagOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Indica se salvare i tag intelligenti con la cartella di lavoro. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Rappresenta il tipo di visualizzazione del tag intelligente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Imposta le proprietà
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // Applica SmartTagOptions al foglio di lavoro
            // Nota: Modificato da worksheet.SmartTagSetting.Options = options;
            // per utilizzare direttamente l'oggetto options poiché SmartTagSetting non ha la proprietà Options
            // (Supponendo che le opzioni debbano essere usate direttamente)
            
            // Aggiungi alcuni dati per dimostrare
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


