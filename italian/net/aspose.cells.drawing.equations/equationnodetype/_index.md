---
title: "Enum EquationNodeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Equations.EquationNodeType. Tipo di nodo equazione. Nota 1199 Attualmente c'è un solo nodo nello scope e il suo valore enumerativo è 1. Il nodo specificato è usato per memorizzare testo matematico. 2100199 Indica che il nodo è un componente di alcuni nodi di funzioni speciali. 3200 Indica che il nodo ha alcune funzioni speciali"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Tipo di nodo equazione. Nota: (1)[1-99] Attualmente c'è solo un nodo nell'ambito, e il suo valore di enumerazione è 1. Il nodo che specifica è utilizzato per memorizzare testo matematico. (2)[100-199] Indica che il nodo è un componente di alcuni nodi di funzioni speciali. (3)[200-] Indica che il nodo ha alcune funzioni speciali.

```csharp
public enum EquationNodeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| UnKnow | `0` | UnKnow |
| Text | `1` | specifica un nodo che memorizza testo matematico |
| Base | `100` | Specifica un componente Base |
| Denominator | `101` | Specifica un componente Denominator |
| Numerator | `102` | Specifica un componente Numerator |
| FunctionName | `103` | Specifica un componente FunctionName |
| Subscript | `104` | Specifica un componente Subscript |
| Superscript | `105` | Specifica un componente Superscript |
| Degree | `106` | Specifica un componente Degree |
| MatrixRow | `107` | Specifica un componente MatrixRow. Una singola riga della matrice |
| Limit | `108` | Rappresenta un sotto-oggetto della funzione Lower-Limit o Upper-Limit |
| EquationParagraph | `200` | Specifica un paragrafo matematico(oMathPara). |
| MathematicalEquation | `201` | Specifica un'equazione o un'espressione matematica(OMath). |
| FractionEquation | `202` | Specifica un'equazione frazionaria |
| FunctionEquation | `203` | Specifica un'equazione di funzione |
| DelimiterEquation | `204` | Specifica un'equazione delimitatrice |
| NaryEquation | `205` | Specifica un'equazione operatore n-ario |
| RadicalEquation | `206` | Specifica l'equazione radicale |
| SuperscriptEquation | `207` | Specifica un'equazione in apice |
| SubscriptEquation | `208` | Specifica un'equazione in pedice |
| SubSupEquation | `209` | Specifica un'equazione con apici e pedici a destra degli operandi. |
| PreSubSupEquation | `210` | Specifica un'equazione con apici e pedici a sinistra degli operandi. |
| AccentEquation | `211` | Specifica un'equazione di accento |
| BarEquation | `212` | Specifica un'equazione a barra |
| BorderBoxEquation | `213` | Specifica un'equazione di riquadro bordato |
| BoxEquation | `214` | Specifica un'equazione di riquadro |
| GroupCharacterEquation | `215` | Specifica un'equazione Gruppo-Carattere |
| MatrixEquation | `216` | Specifica l'equazione Matrice, |
| LowerLimit | `217` | Specifica la funzione Limite Inferiore |
| UpperLimit | `218` | Specifica la funzione Limite Superiore |
| Mathematical | `201` | Specifica un'equazione o un'espressione matematica(OMath). |
| Fraction | `202` | Specifica un'equazione frazionaria |
| Function | `203` | Specifica un'equazione di funzione |
| Delimiter | `204` | Specifica un'equazione delimitatrice |
| Nary | `205` | Specifica un'equazione operatore n-ario |
| Radical | `206` | Specifica l'equazione radicale |
| Sup | `207` | Specifica un'equazione in apice |
| Sub | `208` | Specifica un'equazione in pedice |
| SubSup | `209` | Specifica un'equazione con apici e pedici a destra degli operandi. |
| PreSubSup | `210` | Specifica un'equazione con apici e pedici a sinistra degli operandi. |
| Accent | `211` | Specifica un'equazione di accento |
| Bar | `212` | Specifica un'equazione a barra |
| BorderBox | `213` | Specifica un'equazione di riquadro bordato |
| Box | `214` | Specifica un'equazione di riquadro |
| GroupChr | `215` | Specifica un'equazione Gruppo-Carattere |
| Matrix | `216` | Specifica l'equazione Matrice, |
| ArrayEquation | `317` | Specifica la funzione Array-Equazioni. La funzione consiste in una o più equazioni. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un'equazione al primo foglio di lavoro
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo matematico dall'equazione
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Crea un nodo di accento con carattere circonflesso
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Aggiungi nodo base e nodo di testo
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Salva la cartella di lavoro
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


