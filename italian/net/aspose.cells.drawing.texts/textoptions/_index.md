---
title: "Classe TextOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.Texts.TextOptions. Rappresenta le opzioni di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/
---
## TextOptions class

Rappresenta le opzioni di testo.

```csharp
public class TextOptions : Font
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor/) { get; set; } | Ottiene e imposta il colore con un valore ARGB a 32 bit.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [CapsType](../../aspose.cells.drawing.texts/textoptions/capstype/) { get; set; } | Ottiene e imposta il tipo di maiuscole per i testi della forma. |
| [Charset](../../aspose.cells/font/charset/) { get; set; } | Rappresenta il set di caratteri.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [Color](../../aspose.cells/font/color/) { get; set; } | Ottiene o imposta il colore del carattere.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [DoubleSize](../../aspose.cells/font/doublesize/) { get; set; } | Ottiene e imposta la dimensione doppia del carattere.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [FarEastName](../../aspose.cells.drawing.texts/textoptions/fareastname/) { get; set; } | Ottiene e imposta il nome FarEast. |
| [Fill](../../aspose.cells.drawing.texts/textoptions/fill/) { get; } | Rappresenta il formato di riempimento del testo. |
| [IsBold](../../aspose.cells/font/isbold/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in grassetto.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [IsItalic](../../aspose.cells/font/isitalic/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in corsivo.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [IsNormalizeHeights](../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) { get; set; } | Indica se la normalizzazione dell'altezza deve essere applicata al segmento di testo. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout/) { get; set; } | Ottiene o imposta un valore che indica se il carattere ha una singola barratura.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [IsSubscript](../../aspose.cells/font/issubscript/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in apice basso.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [IsSuperscript](../../aspose.cells/font/issuperscript/) { get; set; } | Ottiene o imposta un valore che indica se il carattere è in apice alto.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [Kerning](../../aspose.cells.drawing.texts/textoptions/kerning/) { get; set; } | Specifica la dimensione minima del carattere a cui avverrà il kerning dei caratteri per questo segmento di testo. |
| [LanguageCode](../../aspose.cells.drawing.texts/textoptions/languagecode/) { get; set; } | Ottiene e imposta la lingua dell'interfaccia utente. |
| [LatinName](../../aspose.cells.drawing.texts/textoptions/latinname/) { get; set; } | Ottiene e imposta il nome latino. |
| override [Name](../../aspose.cells.drawing.texts/textoptions/name/) { get; set; } | Ottiene e imposta il nome della shape. |
| [Outline](../../aspose.cells.drawing.texts/textoptions/outline/) { get; } | Rappresenta il formato del contorno del testo. |
| [SchemeType](../../aspose.cells/font/schemetype/) { get; set; } | Ottiene e imposta il tipo di schema del carattere.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [ScriptOffset](../../aspose.cells/font/scriptoffset/) { get; set; } | Ottiene e imposta lo spostamento dello script,in unità di percentuale(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [Shadow](../../aspose.cells.drawing.texts/textoptions/shadow/) { get; } | Rappresenta un oggetto [`ShadowEffect`](../../aspose.cells.drawing/shadoweffect/) che specifica l'effetto ombra per l'elemento del grafico o la forma. |
| [Size](../../aspose.cells/font/size/) { get; set; } | Ottiene o imposta la dimensione del carattere.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [Spacing](../../aspose.cells.drawing.texts/textoptions/spacing/) { get; set; } | Specifica la spaziatura tra i caratteri all'interno di un segmento di testo. |
| [StrikeType](../../aspose.cells/font/striketype/) { get; set; } | Ottiene il tipo di barratura del testo.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [ThemeColor](../../aspose.cells/font/themecolor/) { get; set; } | Ottiene e imposta il colore del tema.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [Underline](../../aspose.cells/font/underline/) { get; set; } | Ottiene o imposta il tipo di sottolineatura del carattere.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [UnderlineColor](../../aspose.cells.drawing.texts/textoptions/underlinecolor/) { get; set; } | Ottiene o imposta il colore della sottolineatura. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Equals](../../aspose.cells/font/equals/)(Font) | Verifica se due font sono uguali.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| [SetName](../../aspose.cells/font/setname/)(string, FontSchemeType) | Imposta il nome e lo schema del font.(Ereditato da [`Font`](../../aspose.cells/font/).) |
| override [ToString](../../aspose.cells/font/tostring/)() | Restituisce una stringa che rappresenta l'oggetto Cell corrente.(Ereditato da [`Font`](../../aspose.cells/font/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma al foglio di lavoro con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            
            // Aggiungi testo alla forma e ottieni TextOptions
            shape.TextBody.Text = "Sample Text";
            TextOptions textOptions = shape.TextBody[2].TextOptions;
            
            // Imposta le opzioni di testo
            textOptions.Fill.SolidFill.Color = System.Drawing.Color.Red;
            textOptions.Fill.SolidFill.Transparency = 0.5;
            
            // Salva la cartella di lavoro
            workbook.Save("TextOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../aspose.cells/font/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


