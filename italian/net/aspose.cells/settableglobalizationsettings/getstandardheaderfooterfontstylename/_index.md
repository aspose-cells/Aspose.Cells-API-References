---
title: "SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SettableGlobalizationSettings. Ottiene il nome dello stile di carattere standard inglese Regular Bold Italic per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito"
type: docs
url: /it/net/aspose.cells/settableglobalizationsettings/getstandardheaderfooterfontstylename/
---
## SettableGlobalizationSettings.GetStandardHeaderFooterFontStyleName method

Ottiene il nome standard dello stile di carattere inglese (Regular, Bold, Italic) per Intestazione/Piè di pagina in base al nome dello stile di carattere locale fornito.

```csharp
public override string GetStandardHeaderFooterFontStyleName(string localfontStyleName)
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

    public class SettableGlobalizationSettingsMethodGetStandardHeaderFooterFontStyleNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea impostazioni di globalizzazione personalizzate
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Imposta una mappatura del nome dello stile di carattere standard per intestazione/piè di pagina
            settings.SetStandardHeaderFooterFontStyleName("MyLocalFontStyle", "Arial");

            // Applica le impostazioni alla cartella di lavoro
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Chiama il metodo GetStandardHeaderFooterFontStyleName con un nome di stile di carattere locale
                string standardFontStyle = settings.GetStandardHeaderFooterFontStyleName("MyLocalFontStyle");
                
                // Visualizza il risultato
                Console.WriteLine($"Standard font style name for 'MyLocalFontStyle': {standardFontStyle}");

                // Crea un'intestazione con il nome di stile di carattere locale
                worksheet.PageSetup.SetHeader(1, "&\"MyLocalFontStyle\"&12Test Header");

                // Mostra l'effetto nel foglio di calcolo
                Console.WriteLine("Header set with local font style name 'MyLocalFontStyle'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardHeaderFooterFontStyleName method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetStandardHeaderFooterFontStyleNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


