---
title: "MsoFillFormatHelper.BackColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormatHelper. Ottiene e imposta il colore di sfondo del file"
type: docs
url: /it/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Ottiene e imposta il colore di sfondo del file.

```csharp
public Color BackColor { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'etichetta solo per avere del contenuto nel foglio
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper non espone un costruttore pubblico, usa la reflection per istanziarlo
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Imposta BackColor a un colore noto (ad es., LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Leggi nuovamente il valore di BackColor e visualizzalo
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Facoltativamente puoi anche leggere ForeColor per mostrare che rimane predefinito
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Salva la cartella di lavoro – il fill helper non è collegato a una forma,
                // ma il salvataggio dimostra che il codice è stato eseguito senza errori.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


