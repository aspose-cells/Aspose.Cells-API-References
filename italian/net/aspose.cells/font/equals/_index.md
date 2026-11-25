---
title: "Font.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Font. Verifica se due caratteri sono uguali"
type: docs
url: /it/net/aspose.cells/font/equals/
---
## Font.Equals method

Verifica se due caratteri sono uguali.

```csharp
public bool Equals(Font font)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| font | Font | Oggetto font confrontato. |

### Valore di ritorno

Vero se uguale all'oggetto font confrontato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea due oggetti font da confrontare
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Chiama il metodo Equals per confrontare i font
                bool areEqual = font1.Equals(font2);

                // Visualizza il risultato
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Modifica un font per renderli diversi
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


