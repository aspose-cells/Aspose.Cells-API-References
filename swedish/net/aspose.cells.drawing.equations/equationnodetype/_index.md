---
title: "Enum EquationNodeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Equations.EquationNodeType enum. Ekvationsnodtyp. Observera 1199 För närvarande finns det bara en nod i omfattningen och dess uppräkningsvärde är 1. Noden den specificerar används för att lagra matematisk text. 2100199 Indikerar att noden är en komponent av vissa specialfunktioner. 3200 Indikerar att noden har vissa specialfunktioner"
type: docs
url: /sv/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Ekvationsnodtyp. Observera: (1)[1-99] För närvarande finns det bara en nod i omfånget, och dess uppräkningsvärde är 1. Noden den specificerar används för att lagra matematisk text. (2)[100-199] Indikerar att noden är en komponent i vissa specialfunktion‑noder. (3)[200-] Indikerar att noden har vissa specialfunktioner.

```csharp
public enum EquationNodeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| UnKnow | `0` | Okänd |
| Text | `1` | specificerar en nod som lagrar matematisk text |
| Base | `100` | Specificerar en Bas-komponent |
| Denominator | `101` | Specificerar en Nämnare-komponent |
| Numerator | `102` | Specificerar en Täljare-komponent |
| FunctionName | `103` | Specificerar en Funktionsnamn-komponent |
| Subscript | `104` | Specificerar en Nedsänkt komponent |
| Superscript | `105` | Specificerar en Upphöjd komponent |
| Degree | `106` | Specificerar en Grad-komponent |
| MatrixRow | `107` | Specificerar en MatrixRow-komponent. En enda rad i matrisen |
| Limit | `108` | Representerar ett underobjekt av Lower-Limit-funktion eller Upper-Limit-funktion |
| EquationParagraph | `200` | Specificerar ett matematiskt stycke (oMathPara). |
| MathematicalEquation | `201` | Specificerar en ekvation eller ett matematiskt uttryck (OMath). |
| FractionEquation | `202` | Specificerar en bråkequation |
| FunctionEquation | `203` | Specificerar en funktionsekvation |
| DelimiterEquation | `204` | Specificerar en avgränsareekvation |
| NaryEquation | `205` | Specificerar en n-är operator-ekvation |
| RadicalEquation | `206` | Specificerar radikalekvationen |
| SuperscriptEquation | `207` | Specificerar en upphöjd ekvation |
| SubscriptEquation | `208` | Specificerar en nedsänkt ekvation |
| SubSupEquation | `209` | Specificerar en ekvation med upphöjda och nedsänkta element till höger om operanderna. |
| PreSubSupEquation | `210` | Specificerar en ekvation med upphöjda och nedsänkta element till vänster om operanderna. |
| AccentEquation | `211` | Specificerar en accentekvation |
| BarEquation | `212` | Specificerar stapelsekvation |
| BorderBoxEquation | `213` | Specificerar kantboxekvation |
| BoxEquation | `214` | Specificerar boxekvation |
| GroupCharacterEquation | `215` | Specificerar grupp-teckenekvation |
| MatrixEquation | `216` | Specificerar matrisekvationen, |
| LowerLimit | `217` | Specificerar funktionen nedre gräns |
| UpperLimit | `218` | Specificerar funktionen övre gräns |
| Mathematical | `201` | Specificerar en ekvation eller ett matematiskt uttryck (OMath). |
| Fraction | `202` | Specificerar en bråkequation |
| Function | `203` | Specificerar en funktionsekvation |
| Delimiter | `204` | Specificerar en avgränsareekvation |
| Nary | `205` | Specificerar en n-är operator-ekvation |
| Radical | `206` | Specificerar radikalekvationen |
| Sup | `207` | Specificerar en upphöjd ekvation |
| Sub | `208` | Specificerar en nedsänkt ekvation |
| SubSup | `209` | Specificerar en ekvation med upphöjda och nedsänkta element till höger om operanderna. |
| PreSubSup | `210` | Specificerar en ekvation med upphöjda och nedsänkta element till vänster om operanderna. |
| Accent | `211` | Specificerar en accentekvation |
| Bar | `212` | Specificerar stapelsekvation |
| BorderBox | `213` | Specificerar kantboxekvation |
| Box | `214` | Specificerar boxekvation |
| GroupChr | `215` | Specificerar grupp-teckenekvation |
| Matrix | `216` | Specificerar matrisekvationen, |
| ArrayEquation | `317` | Specificerar ekvationsarray-funktionen. Funktionen består av en eller flera ekvationer. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationNodeTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en ekvation i det första kalkylbladet
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hämta matematiknoden från ekvationen
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Skapa en accentnod med cirkumflextecken
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Lägg till basnod och textnod
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Spara arbetsboken
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


