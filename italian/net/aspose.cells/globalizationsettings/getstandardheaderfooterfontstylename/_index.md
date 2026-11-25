---
title: "GlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GlobalizationSettings. Ottiene il nome dello stile di carattere standard inglese Regular Bold Italic per Header/Footer secondo il nome dello stile di carattere locale fornito"
type: docs
url: /it/net/aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename/
---
## GlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Ottiene il nome standard dello stile di carattere inglese (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito.

```csharp
public virtual string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| localfontStyleName | String | Nome dello stile di carattere locale per Intestazione/Piè di pagina. |

### Valore di ritorno

Nome dello stile di carattere standard inglese (Regular, Bold, Italic)

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di impostazioni di globalizzazione personalizzate
            var globalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Dimostra la chiamata al metodo con tipo di parametro (String)
                string localStyle = "CustomBold";
                string standardStyle = globalizationSettings.GetStandardHeaderFooterFontStyleName(localStyle);
                Console.WriteLine($"Converted font style: {localStyle} -> {standardStyle}");

                // Applica le impostazioni di globalizzazione alla cartella di lavoro
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Imposta l'intestazione con stile di carattere personalizzato che sarà convertito
                // Usa il metodo SetHeader con il parametro sezione (0 = sinistra, 1 = centro, 2 = destra)
                worksheet.PageSetup.SetHeader(1, "&\"Arial\"&\"CustomBold\"&12Header Text");

                // Salva la cartella di lavoro per mostrare l'effetto
                workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
        }
    }

    // Implementazione delle impostazioni di globalizzazione personalizzate
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
        {
            // Converti i nomi di stili di carattere personalizzati in nomi standard
            return localfontStyleName switch
            {
                "CustomBold" => "Bold",
                "CustomItalic" => "Italic",
                _ => base.GetStandardHeaderFooterFontStyleName(localfontStyleName)
            };
        }
    }
}
```

### Vedi anche

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


