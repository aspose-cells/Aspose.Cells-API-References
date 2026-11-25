---
title: "Cell.GetCharacters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo della cella"
type: docs
url: /it/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo della cella.

```csharp
public FontSetting[] GetCharacters()
```

### Valore di ritorno

Tutti gli oggetti Characters

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta testo formattato in HTML nella cella A1 con diverse parti di formattazione
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Ottieni le informazioni di formattazione dei caratteri dalla cella A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Emetti le informazioni di formattazione
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo della cella.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flag | Booleano | Indica se applicare lo stile tabella alla cella se la cella è nella tabella. |

### Valore di ritorno

Tutti gli oggetti Characters

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi testo alla cella C8 con formattazione
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Formatta le parti del testo
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Ottieni tutte le impostazioni dei caratteri con la formattazione
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Visualizza i colori dei caratteri
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


