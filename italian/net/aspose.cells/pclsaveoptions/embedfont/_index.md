---
title: "PclSaveOptions.EmbedFont"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PclSaveOptions. Indica se incorporare il carattere nel file Pcl di output"
type: docs
url: /it/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Indica se incorporare il font nel file Pcl di output.

```csharp
public bool EmbedFont { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e aggiungi alcuni dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Crea opzioni di salvataggio PCL
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Leggi e visualizza il valore corrente della proprietà EmbedFont
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Opzionale) Se la proprietà è scrivibile puoi impostarla, ma qui la leggiamo solo.
                // pclOptions.EmbedFont = true;

                // Salva la cartella di lavoro come file PCL utilizzando le opzioni
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


