---
title: "Classe FontSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.FontSetting. Rappresenta un intervallo di caratteri nel testo della cella"
type: docs
url: /it/net/aspose.cells/fontsetting/
---
## FontSetting class

Rappresenta un intervallo di caratteri all'interno del testo della cella.

```csharp
public class FontSetting
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Restituisce il font di questo oggetto. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ottiene la lunghezza dei caratteri. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ottiene l'indice iniziale dei caratteri. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Restituisce le opzioni di testo. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Ottiene il tipo di nodo di testo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Imposta lo stile predefinito di WordArt. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            workbook.Worksheets.Add();

            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedere alla cella "A1" dal foglio di lavoro
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Visit Aspose!");

            // Ottenimento dell'intervallo di caratteri
            FontSetting character = cell.Characters(6, 7);

            // Impostazione del font dei caratteri selezionati in grassetto
            character.Font.IsBold = true;

            // Impostazione del colore del font dei caratteri selezionati in blu
            character.Font.Color = Color.Blue;

            // Salvataggio del file Excel
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


