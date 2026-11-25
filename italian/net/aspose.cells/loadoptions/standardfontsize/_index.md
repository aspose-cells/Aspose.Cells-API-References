---
title: "LoadOptions.StandardFontSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Imposta la dimensione predefinita del carattere standard"
type: docs
url: /it/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Imposta la dimensione predefinita del carattere standard.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare DefaultStyleSettings. Questa proprietà sarà rimossa tra 12 mesi a partire da marzo 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // Crea le opzioni di caricamento HTML e imposta StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Carica la cartella di lavoro con le opzioni
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Accedi al primo foglio di lavoro e alle celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Imposta del testo di esempio e verifica le proprietà del carattere
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


