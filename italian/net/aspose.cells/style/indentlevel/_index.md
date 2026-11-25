---
title: "Style.IndentLevel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250"
type: docs
url: /it/net/aspose.cells/style/indentlevel/
---
## Style.IndentLevel property

Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250.

```csharp
public int IndentLevel { get; set; }
```

### Osservazioni

Se il tipo di allineamento orizzontale del testo è impostato su un valore diverso da sinistra o destra, il livello di rientro verrà azzerato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIndentLevelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta diversi livelli di rientro per le celle
            for (int i = 0; i < 16; i++)
            {
                Cell cell = cells[i, 0];
                Style style = cell.GetStyle();
                style.IndentLevel = i;
                style.HorizontalAlignment = TextAlignmentType.Left;
                cell.SetStyle(style);
                cell.PutValue($"Indent Level {i}");
            }

            // Salva la cartella di lavoro
            workbook.Save("IndentLevelDemo.xlsx");
            Console.WriteLine("Workbook saved with different indent levels.");
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


