---
title: "Klass DelimiterEquationNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.DelimiterEquationNode class. Denna klass specificerar en avgränsarekvation bestående av öppnings- och stängningsavgränsare såsom parenteser, klamrar, hakparenteser och vertikala streck samt en komponent som finns inuti. Avgränsaren kan ha mer än en komponent med ett bestämt separator-tecken mellan varje komponent."
type: docs
url: /sv/net/aspose.cells.drawing.equations/delimiterequationnode/
---
## DelimiterEquationNode class

Denna klass specificerar avgränsarekvationen, bestående av öppnings‑ och stängningsavgränsare (såsom parenteser, klammerparenteser, hakparenteser och vertikala streck) samt en komponent som finns inuti. Avgränsaren kan ha mer än en komponent, med ett angivet separator‑tecken mellan varje komponent.

```csharp
public class DelimiterEquationNode : EquationNode
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BeginChar](../../aspose.cells.drawing.equations/delimiterequationnode/beginchar/) { get; set; } | Avgränsningens starttecken. |
| [DelimiterShape](../../aspose.cells.drawing.equations/delimiterequationnode/delimitershape/) { get; set; } | Specificerar formen på avgränsare i avgränsningsobjektet. |
| [EndChar](../../aspose.cells.drawing.equations/delimiterequationnode/endchar/) { get; set; } | Avgränsningens sluttecken. |
| [EquationType](../../aspose.cells.drawing.equations/equationnode/equationtype/) { get; } | Hämta ekvationstypen för den aktuella noden (ärvd från [`EquationNode`](../equationnode/).) |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Returnerar teckensnittet för detta objekt. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Hämtar längden på tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [NaryGrow](../../aspose.cells.drawing.equations/delimiterequationnode/narygrow/) { get; set; } | Specificerar om avgränsaren automatiskt ska expandera och kontrahera med formelns höjd. |
| [ParentNode](../../aspose.cells.drawing.equations/equationnode/parentnode/) { get; set; } | Anger föräldranoden för den aktuella noden (Ärvt från [`EquationNode`](../equationnode/).) |
| [SeparatorChar](../../aspose.cells.drawing.equations/delimiterequationnode/separatorchar/) { get; set; } | Avgränsare separator-tecken. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Hämtar startindexet för tecknen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Returnerar textalternativen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.equations/equationnode/type/) { get; } | Representerar nodens typ. (Ärvt från [`EquationNode`](../equationnode/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNode) | Infogar den angivna noden i slutet av den aktuella nodens lista över barnnoder. (Ärvt från [`EquationNode`](../equationnode/).) |
| [AddChild](../../aspose.cells.drawing.equations/equationnode/addchild/)(EquationNodeType) | Infoga en nod av den angivna typen i slutet av barnnodlistan för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| override [Equals](../../aspose.cells.drawing.equations/delimiterequationnode/equals/)(object) | Bestäm om den aktuella ekvationsnoden är lika med den angivna noden |
| [GetChild](../../aspose.cells.drawing.equations/equationnode/getchild/)(int) | Returnerar noden på det angivna indexet bland den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertAfter](../../aspose.cells.drawing.equations/equationnode/insertafter/)(EquationNodeType) | Infogar den angivna noden efter den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertBefore](../../aspose.cells.drawing.equations/equationnode/insertbefore/)(EquationNodeType) | Infogar den angivna noden före den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [InsertChild](../../aspose.cells.drawing.equations/equationnode/insertchild/)(int, EquationNodeType) | Infogar en nod av den angivna typen på den angivna indexpositionen i den aktuella nodens barnnodlista. (Ärvt från [`EquationNode`](../equationnode/).) |
| [Remove](../../aspose.cells.drawing.equations/equationnode/remove/)() | Tar bort sig själv från föräldern. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveAllChildren](../../aspose.cells.drawing.equations/equationnode/removeallchildren/)() | Tar bort alla barnnoder för den aktuella noden. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(EquationNode) | Tar bort den angivna noden från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [RemoveChild](../../aspose.cells.drawing.equations/equationnode/removechild/)(int) | Tar bort noden på det angivna indexet från den aktuella nodens barn. (Ärvt från [`EquationNode`](../equationnode/).) |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Ställer in den förinställda WordArt‑stilen. (Ärvt från [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [ToLaTeX](../../aspose.cells.drawing.equations/equationnode/tolatex/)() | Konvertera denna ekvation till ett LaTeX‑uttryck. (Ärvt från [`EquationNode`](../equationnode/).) |
| [ToMathML](../../aspose.cells.drawing.equations/equationnode/tomathml/)() | Konvertera denna ekvation till MathML-uttryck.(Härledd från [`EquationNode`](../equationnode/).) |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassDelimiterEquationNodeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Skapa en avgränsningsnod med anpassade inställningar
            DelimiterEquationNode node = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            node.DelimiterShape = EquationDelimiterShapeType.Match;
            node.NaryGrow = false;
            node.SeparatorChar = "!";
            node.BeginChar = "#";
            node.EndChar = "*";

            // Lägg till ett bråk som basinnehåll
            EquationNode baseNode = node.AddChild(EquationNodeType.Base);
            FractionEquationNode fraction = (FractionEquationNode)baseNode.AddChild(EquationNodeType.Fraction);

            // Lägg till täljare
            EquationComponentNode numerator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Numerator);
            TextRunEquationNode textRun = (TextRunEquationNode)numerator.AddChild(EquationNodeType.Text);
            textRun.Text = "A";

            // Lägg till nämnare
            EquationComponentNode denominator = (EquationComponentNode)fraction.AddChild(EquationNodeType.Denominator);
            textRun = (TextRunEquationNode)denominator.AddChild(EquationNodeType.Text);
            textRun.Text = "B";

            // Lägg till en annan basnod med text
            baseNode = node.AddChild(EquationNodeType.Base);
            textRun = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textRun.Text = "a";

            // Spara arbetsboken
            workbook.Save("DelimiterEquationNodeDemo.xlsx");
        }
    }
}
```

### Se även

* class [EquationNode](../equationnode/)
* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


