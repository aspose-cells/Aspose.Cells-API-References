---
title: "Classe DefaultStyleSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.DefaultStyleSettings class. Impostazioni per i valori predefiniti delle proprietà di stile delle cartelle di lavoro"
type: docs
url: /it/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Impostazioni per i valori predefiniti delle proprietà di stile della cartella di lavoro.

```csharp
public class DefaultStyleSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Indica se la proprietà per il formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. Il valore predefinito è false, il che significa che per impostazione predefinita verrà utilizzato il modello personalizzato per formattare i valori finché non è vuoto per uno stile. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Ottiene/Imposta il nome del carattere predefinito per la cartella di lavoro |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Ottiene/Imposta la dimensione del carattere standard predefinita per la cartella di lavoro. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Ottiene/Imposta il valore predefinito per l'allineamento orizzontale |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Ottiene/Imposta il valore predefinito per l'allineamento verticale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle impostazioni di stile predefinite della cartella di lavoro
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Impostazione delle proprietà
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Applica le impostazioni di stile predefinite al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Salva la cartella di lavoro
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


