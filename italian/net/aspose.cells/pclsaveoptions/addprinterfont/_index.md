---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PclSaveOptions. Aggiunge informazioni sul carattere già inserito nella stampante dal produttore"
type: docs
url: /it/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Aggiunge informazioni sul font già aggiunto alla stampante dal produttore.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFullName | String | Nome completo del carattere (ad es. "Times New Roman Bold Italic") utilizzato nel file sorgente. |
| fontPclName | String | Nome del carattere che verrà utilizzato nel documento Pcl di output. |

### Osservazioni

Ci sono 52 caratteri che devono essere incorporati in qualsiasi stampante secondo la specifica Pcl. Tuttavia i produttori possono aggiungere altri caratteri ai loro dispositivi.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi del testo al foglio di lavoro per dimostrare l'uso del carattere
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Crea opzioni di salvataggio PCL
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Chiama il metodo AddPrinterFont con nomi di carattere specifici
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Salva la cartella di lavoro con le opzioni PCL
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


