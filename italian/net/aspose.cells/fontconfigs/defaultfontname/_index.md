---
title: "FontConfigs.DefaultFontName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontConfigs. Ottiene o imposta il nome del carattere predefinito"
type: docs
url: /it/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Ottiene o imposta il nome del carattere predefinito.

```csharp
public static string DefaultFontName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza il nome del carattere predefinito corrente
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Imposta un nuovo nome del carattere predefinito
            FontConfigs.DefaultFontName = "Arial";

            // Crea uno stile senza impostare un carattere esplicito per dimostrare l'uso del carattere predefinito
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Verifica che il carattere sia stato applicato correttamente
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Vedi anche

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


