---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DefaultStyleSettings. Indica se la proprietà per il formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. Il valore predefinito è false, il che significa che per impostazione predefinita verrà utilizzato il modello personalizzato per formattare i valori, a condizione che non sia vuoto per uno stile."
type: docs
url: /it/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indica se la proprietà per il formato numerico è preferibile quando lo stile definisce sia un numero incorporato sia un modello personalizzato. Il valore predefinito è false, il che significa che per impostazione predefinita verrà utilizzato il modello personalizzato per formattare i valori finché non è vuoto per uno stile.

```csharp
public bool BuiltInPreference { get; set; }
```

### Osservazioni

Durante il caricamento di una cartella di lavoro da un file modello esistente, è possibile che per uno stile siano definiti sia il numero incorporato sia il modello personalizzato. Questa proprietà determina se utilizzare il numero incorporato o il modello personalizzato durante la formattazione dei valori con lo stile.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni di stile predefinite
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Dimostra la proprietà BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Applica al foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Salva la cartella di lavoro
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


