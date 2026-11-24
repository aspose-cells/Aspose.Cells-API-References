---
title: "Aufzählung EquationNodeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationNodeType-Enum. Knotentyp. Hinweis 1199 Derzeit gibt es nur einen Knoten im Geltungsbereich und sein Enumerationswert ist 1. Der von ihm spezifizierte Knoten wird verwendet, um mathematischen Text zu speichern. 2100199 Gibt an, dass der Knoten ein Bestandteil einiger spezieller Funktionsknoten ist. 3200 Gibt an, dass der Knoten einige spezielle Funktionen hat"
type: docs
url: /de/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Gleichungsknotentyp. Hinweis: (1)[1-99] Derzeit gibt es nur einen Knoten im Geltungsbereich, und sein Enumerationswert ist 1. Der von ihm spezifizierte Knoten wird verwendet, um mathematischen Text zu speichern. (2)[100-199] Gibt an, dass der Knoten ein Bestandteil einiger spezieller Funktionsknoten ist. (3)[200-] Gibt an, dass der Knoten einige Sonderfunktionen hat.

```csharp
public enum EquationNodeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| UnKnow | `0` | Unbekannt |
| Text | `1` | gibt einen Knoten an, der mathematischen Text speichert |
| Base | `100` | Gibt eine Basis-Komponente an |
| Denominator | `101` | Gibt eine Nenner-Komponente an |
| Numerator | `102` | Gibt eine Zähler-Komponente an |
| FunctionName | `103` | Gibt eine FunctionName-Komponente an |
| Subscript | `104` | Gibt eine Subscript-Komponente an |
| Superscript | `105` | Gibt eine Superscript-Komponente an |
| Degree | `106` | Gibt eine Degree-Komponente an |
| MatrixRow | `107` | Gibt eine MatrixRow-Komponente an. Eine einzelne Zeile der Matrix |
| Limit | `108` | Stellt ein Unterobjekt der Lower-Limit- oder Upper-Limit-Funktion dar |
| EquationParagraph | `200` | Gibt einen mathematischen Absatz (oMathPara) an. |
| MathematicalEquation | `201` | Gibt eine Gleichung oder mathematischen Ausdruck (OMath) an. |
| FractionEquation | `202` | Gibt eine Bruchgleichung an |
| FunctionEquation | `203` | Gibt eine Funktionsgleichung an |
| DelimiterEquation | `204` | Gibt eine Trennzeichen-Gleichung an |
| NaryEquation | `205` | Gibt eine n-äre Operator-Gleichung an |
| RadicalEquation | `206` | Gibt die Radikalgleichung an |
| SuperscriptEquation | `207` | Gibt eine Superscript-Gleichung an |
| SubscriptEquation | `208` | Gibt eine Subscript-Gleichung an |
| SubSupEquation | `209` | Gibt eine Gleichung mit Superscripts und Subscripts rechts von den Operanden an. |
| PreSubSupEquation | `210` | Gibt eine Gleichung mit Superscripts und Subscripts links von den Operanden an. |
| AccentEquation | `211` | Gibt die Akzentgleichung an |
| BarEquation | `212` | Gibt die Balkengleichung an |
| BorderBoxEquation | `213` | Gibt die Randbox-Gleichung an |
| BoxEquation | `214` | Gibt die Box-Gleichung an |
| GroupCharacterEquation | `215` | Gibt die Gruppenzeichen-Gleichung an |
| MatrixEquation | `216` | Gibt die Matrixgleichung an, |
| LowerLimit | `217` | Gibt die Untergrenzenfunktion an |
| UpperLimit | `218` | Gibt die Obergrenzenfunktion an |
| Mathematical | `201` | Gibt eine Gleichung oder mathematischen Ausdruck (OMath) an. |
| Fraction | `202` | Gibt eine Bruchgleichung an |
| Function | `203` | Gibt eine Funktionsgleichung an |
| Delimiter | `204` | Gibt eine Trennzeichen-Gleichung an |
| Nary | `205` | Gibt eine n-äre Operator-Gleichung an |
| Radical | `206` | Gibt die Radikalgleichung an |
| Sup | `207` | Gibt eine Superscript-Gleichung an |
| Sub | `208` | Gibt eine Subscript-Gleichung an |
| SubSup | `209` | Gibt eine Gleichung mit Superscripts und Subscripts rechts von den Operanden an. |
| PreSubSup | `210` | Gibt eine Gleichung mit Superscripts und Subscripts links von den Operanden an. |
| Accent | `211` | Gibt die Akzentgleichung an |
| Bar | `212` | Gibt die Balkengleichung an |
| BorderBox | `213` | Gibt die Randbox-Gleichung an |
| Box | `214` | Gibt die Box-Gleichung an |
| GroupChr | `215` | Gibt die Gruppenzeichen-Gleichung an |
| Matrix | `216` | Gibt die Matrixgleichung an, |
| ArrayEquation | `317` | Gibt die Gleichungsarray-Funktion an. Die Funktion besteht aus einer oder mehreren Gleichungen. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge eine Gleichung zum ersten Arbeitsblatt hinzu
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Hole den Mathematik-Knoten aus der Gleichung
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Erstelle einen Akzentknoten mit Zirkumflexzeichen
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Füge Basis-Knoten und Text-Knoten hinzu
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Speichere die Arbeitsmappe
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


