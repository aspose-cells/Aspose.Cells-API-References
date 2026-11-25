---
title: "Cell.SetCharacters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Imposta il formato di testo ricco della cella"
type: docs
url: /it/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Imposta il formato rich text della cella.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| caratteri | FontSetting[] | Tutti gli oggetti Characters. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Imposta il valore della cella per applicare la formattazione di testo avanzato
            cell.Value = "Hello World!";

            try
            {
                // Crea impostazioni di carattere per diverse parti del testo
                FontSetting[] fontSettings = new FontSetting[2];

                // Formatta i primi 5 caratteri (Hello) in grassetto rosso
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Formatta i caratteri rimanenti ( World!) in corsivo blu
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Applica le impostazioni di carattere formattate usando SetCharacters
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


