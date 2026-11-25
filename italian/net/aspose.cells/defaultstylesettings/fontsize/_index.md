---
title: "DefaultStyleSettings.FontSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DefaultStyleSettings. Ottiene/Imposta la dimensione del carattere standard predefinita per la cartella di lavoro"
type: docs
url: /it/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Ottiene/Imposta la dimensione del carattere standard predefinita per la cartella di lavoro.

```csharp
public double FontSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Imposta il nome e la dimensione del carattere predefiniti
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Carica il file HTML con queste impostazioni
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Accedi a una cella e visualizza la sua dimensione del carattere
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Vedi anche

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


