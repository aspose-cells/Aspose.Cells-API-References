---
title: "Énumération EquationNodeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationNodeType enum. Type de nœud d'équation. Remarque 1199 Actuellement il n'y a qu'un seul nœud dans la portée et sa valeur d'énumération est 1. Le nœud qu'il spécifie est utilisé pour stocker du texte mathématique. 2100199 Indique que le nœud est un composant de certains nœuds de fonctions spéciales. 3200 Indique que le nœud possède certaines fonctions spéciales"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationnodetype/
---
## EquationNodeType enumeration

Type de nœud d'équation. Remarque : (1)[1-99] Il n'y a actuellement qu'un seul nœud dans la portée, et sa valeur d'énumération est 1. Le nœud qu'il spécifie est utilisé pour stocker du texte mathématique. (2)[100-199] Indique que le nœud est un composant de certains nœuds de fonctions spéciales. (3)[200-] Indique que le nœud possède des fonctions spéciales.

```csharp
public enum EquationNodeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| UnKnow | `0` | Inconnu |
| Text | `1` | spécifie un nœud qui stocke du texte mathématique |
| Base | `100` | Spécifie un composant Base |
| Denominator | `101` | Spécifie un composant Denominator |
| Numerator | `102` | Spécifie un composant Numerator |
| FunctionName | `103` | Spécifie un composant FunctionName |
| Subscript | `104` | Spécifie un composant Subscript |
| Superscript | `105` | Spécifie un composant Superscript |
| Degree | `106` | Spécifie un composant Degree |
| MatrixRow | `107` | Spécifie un composant MatrixRow. Une seule ligne de la matrice |
| Limit | `108` | Représente un sous-objet de la fonction Lower-Limit ou de la fonction Upper-Limit |
| EquationParagraph | `200` | Spécifie un paragraphe mathématique(oMathPara). |
| MathematicalEquation | `201` | Spécifie une équation ou une expression mathématique(OMath). |
| FractionEquation | `202` | Spécifie une équation fractionnaire |
| FunctionEquation | `203` | Spécifie une équation fonctionnelle |
| DelimiterEquation | `204` | Spécifie une équation délimiteur |
| NaryEquation | `205` | Spécifie une équation d'opérateur n-aire |
| RadicalEquation | `206` | Spécifie l'équation radicale |
| SuperscriptEquation | `207` | Spécifie une équation en exposant |
| SubscriptEquation | `208` | Spécifie une équation en indice |
| SubSupEquation | `209` | Spécifie une équation avec des exposants et des indices à droite des opérandes. |
| PreSubSupEquation | `210` | Spécifie une équation avec des exposants et des indices à gauche des opérandes. |
| AccentEquation | `211` | Spécifie une équation d'accent |
| BarEquation | `212` | Spécifie une équation à barre |
| BorderBoxEquation | `213` | Spécifie une équation de boîte bordure |
| BoxEquation | `214` | Spécifie une équation de boîte |
| GroupCharacterEquation | `215` | Spécifie une équation de groupe-caractère |
| MatrixEquation | `216` | Spécifie l'équation de matrice, |
| LowerLimit | `217` | Spécifie la fonction de limite inférieure |
| UpperLimit | `218` | Spécifie la fonction de limite supérieure |
| Mathematical | `201` | Spécifie une équation ou une expression mathématique(OMath). |
| Fraction | `202` | Spécifie une équation fractionnaire |
| Function | `203` | Spécifie une équation fonctionnelle |
| Delimiter | `204` | Spécifie une équation délimiteur |
| Nary | `205` | Spécifie une équation d'opérateur n-aire |
| Radical | `206` | Spécifie l'équation radicale |
| Sup | `207` | Spécifie une équation en exposant |
| Sub | `208` | Spécifie une équation en indice |
| SubSup | `209` | Spécifie une équation avec des exposants et des indices à droite des opérandes. |
| PreSubSup | `210` | Spécifie une équation avec des exposants et des indices à gauche des opérandes. |
| Accent | `211` | Spécifie une équation d'accent |
| Bar | `212` | Spécifie une équation à barre |
| BorderBox | `213` | Spécifie une équation de boîte bordure |
| Box | `214` | Spécifie une équation de boîte |
| GroupChr | `215` | Spécifie une équation de groupe-caractère |
| Matrix | `216` | Spécifie l'équation de matrice, |
| ArrayEquation | `317` | Spécifie la fonction Equation-Array. La fonction consiste en une ou plusieurs équations. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une équation à la première feuille de calcul
            var equationShape = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenez le nœud mathématique de l'équation
            EquationNode mathNode = equationShape.GetEquationParagraph().GetChild(0);

            // Créez un nœud d'accent avec le caractère circonflexe
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            accentNode.AccentCharacter = "\u0302";

            // Ajoutez le nœud de base et le nœud de texte
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "x";

            // Enregistrez le classeur
            workbook.Save("EquationNodeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


