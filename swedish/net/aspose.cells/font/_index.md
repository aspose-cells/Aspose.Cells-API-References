---
title: Font
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in teckensnittsobjektet som används i ett kalkylblad.
type: docs
weight: 3490
url: /sv/net/aspose.cells/font/
---
## Font class

Kapslar in teckensnittsobjektet som används i ett kalkylblad.

```csharp
public class Font
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ArgbColor](../../aspose.cells/font/argbcolor) { get; set; } | Hämtar och ställer in färgen med ett 32-bitars ARGB-värde. |
| [CapsType](../../aspose.cells/font/capstype) { get; set; } | Hämtar och ställer in typ av textkapslar. |
| [Charset](../../aspose.cells/font/charset) { get; set; } | Representerar teckenuppsättningen. |
| [Color](../../aspose.cells/font/color) { get; set; } | Hämtar eller ställer inColor av teckensnittet. |
| [DoubleSize](../../aspose.cells/font/doublesize) { get; set; } | Hämtar och ställer in den dubbla storleken på teckensnittet. |
| [IsBold](../../aspose.cells/font/isbold) { get; set; } | Hämtar eller ställer in ett värde som anger om teckensnittet är fetstilt. |
| [IsItalic](../../aspose.cells/font/isitalic) { get; set; } | Hämtar eller ställer in ett värde som anger om teckensnittet är kursivt. |
| [IsNormalizeHeights](../../aspose.cells/font/isnormalizeheights) { get; set; } | Indikerar om normaliseringen av höjden som ska tillämpas på texten körs. |
| [IsStrikeout](../../aspose.cells/font/isstrikeout) { get; set; } | Hämtar eller ställer in ett värde som indikerar om teckensnittet är enkel överstruket. |
| [IsSubscript](../../aspose.cells/font/issubscript) { get; set; } | Hämtar eller ställer in ett värde som anger om teckensnittet är nedsänkt. |
| [IsSuperscript](../../aspose.cells/font/issuperscript) { get; set; } | Hämtar eller ställer in ett värde som anger om teckensnittet är superskript. |
| virtual [Name](../../aspose.cells/font/name) { get; set; } | Hämtar eller ställer in namnet på[`Font`](../font) . |
| [SchemeType](../../aspose.cells/font/schemetype) { get; set; } | Hämtar och ställer in schematypen för teckensnittet. |
| [ScriptOffset](../../aspose.cells/font/scriptoffset) { get; set; } | Hämtar och ställer in skriptförskjutningen, i enhet av procent |
| [Size](../../aspose.cells/font/size) { get; set; } | Hämtar eller ställer in storleken på teckensnittet. |
| [StrikeType](../../aspose.cells/font/striketype) { get; set; } | Hämtar strejktypen för texten. |
| [ThemeColor](../../aspose.cells/font/themecolor) { get; set; } | Hämtar och ställer in temafärgen. |
| [Underline](../../aspose.cells/font/underline) { get; set; } | Hämtar eller ställer in teckensnittets understrykningstyp. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Equals](../../aspose.cells/font/equals#equals)(Font) | Kontrollerar om två teckensnitt är lika. |
| override [ToString](../../aspose.cells/font/tostring)() | Returnerar en sträng som representerar det aktuella cellobjektet. |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();

//Hämta referensen till det nyligen tillagda kalkylbladet genom att skicka dess arkindex
Worksheet worksheet = workbook.Worksheets[0];

//Åtkomst till "A1"-cellen från kalkylbladet
Aspose.Cells.Cell cell = worksheet.Cells["A1"];

//Att lägga till något värde i "A1"-cellen
cell.PutValue("Hello Aspose!");

Aspose.Cells.Font font = cell.GetStyle().Font;

//Ställer in teckensnittsnamnet till "Times New Roman"
font.Name = "Times New Roman";

//Ställ in teckenstorlek till 14
font.Size = 14;

//ställer in teckensnittsfärgen som röd
font.Color = System.Drawing.Color.Red;           

//Spara Excel-filen
workbook.Save(@"dest.xls");

[VB.NET]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()

'Få referensen till det nyligen tillagda kalkylbladet genom att skicka dess arkindex
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Accessing the "A1" cell from the worksheet
Dim cell As Aspose.Cells.Cell = worksheet.Cells("A1")

'Adding some value to the "A1" cell
cell.PutValue("Hello Aspose!")

Dim font As Aspose.Cells.Font = cell.GetStyle().Font

'Setting the font name to "Times New Roman"
font.Name = "Times New Roman"

'Ställer in teckenstorlek till 14
font.Size = 14

'ställer in teckensnittsfärgen som röd
font.Color = System.Drawing.Color.Red

'Sparar Excel-filen
workbook.Save("dest.xls")
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
