---
title: "Classe Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Font. Incapsula l'oggetto font utilizzato in un foglio elettronico"
type: docs
url: /it/net/aspose.cells/font/
---
## Font class

Incapsula l'oggetto font utilizzato in un foglio di calcolo.

```csharp
public class Font
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Ottiene e imposta il colore con un valore ARGB a 32 bit. |
| [CapsType](../../aspose.cells/font/capstype/) { get; set; } | (**Obsolete.**) Ottiene e imposta il tipo di maiuscole del testo. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Rappresenta il set di caratteri. |
| [Color](../../aspose.cells/font/color/) { get; set; } | Ottiene o imposta il colore del font. |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Ottiene e imposta la dimensione doppia del carattere. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in grassetto. |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in corsivo. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights/) { get; set; } | (**Obsolete.**) Indica se la normalizzazione dell'altezza da applicare al blocco di testo. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è barrato singolo. |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è pedice. |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è apice. |
| virtual [Name](../../aspose.cells/font/name/) { get; set; } | Ottiene o imposta il nome del `Font`. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Ottiene e imposta il tipo di schema del carattere. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Ottiene e imposta lo spostamento dello script, in unità di percentuale |
| [Size](../../aspose.cells/font/size/) { get; set; } | Ottiene o imposta la dimensione del carattere. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Ottiene il tipo di barratura del testo. |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Ottiene e imposta il colore del tema. |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Ottiene o imposta il tipo di sottolineatura del carattere. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/#equals)(Font) | Verifica se due caratteri sono uguali. |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Imposta il nome e lo schema del carattere. |
| override [ToString](../../aspose.cells/font/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontDemo
    {
        public static void FontExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedere alla cella "A1" dal foglio di lavoro
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Hello Aspose!");

            // Accesso all'oggetto font dello stile della cella
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Impostazione del nome del font a "Times New Roman"
            font.Name = "Times New Roman";

            // Impostazione della dimensione del font a 14
            font.Size = 14;

            // Impostazione del colore del font a Rosso
            font.Color = Color.Red;

            // Impostazione di proprietà aggiuntive del font
            font.IsBold = true;
            font.IsItalic = true;
            font.Underline = FontUnderlineType.Single;
            font.IsStrikeout = false;
            font.IsSuperscript = false;
            font.IsSubscript = false;
            font.Charset = 1;
            font.CapsType = TextCapsType.None;
            font.StrikeType = TextStrikeType.None;
            font.ScriptOffset = 0;
            font.DoubleSize = 14.0;
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            font.ArgbColor = Color.Red.ToArgb();
            font.IsNormalizeHeights = false;
            font.SchemeType = FontSchemeType.None;

            // Salvataggio del file Excel
            workbook.Save("FontExample.xlsx");
            workbook.Save("FontExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


