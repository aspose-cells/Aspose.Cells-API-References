---
title: "Enum EquationMathematicalOperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Equations.EquationMathematicalOperatorType enum. Type d'opérateurs mathématiques"
type: docs
url: /fr/net/aspose.cells.drawing.equations/equationmathematicaloperatortype/
---
## EquationMathematicalOperatorType enumeration

Type d'opérateurs mathématiques

```csharp
public enum EquationMathematicalOperatorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Unknown | `-1` | Utilisez le type inconnu lorsqu'il n'est pas trouvé dans le type existant. |
| ForAll | `0` | "∀" Unicode : \u2200 |
| Complement | `1` | "∁" Unicode : \u2201 |
| PartialDifferential | `2` | "∂" Unicode : \u2202 |
| Exists | `3` | "∃" Unicode : \u2203 |
| NotExists | `4` | "∄" Unicode : \u2204 |
| EmptySet | `5` | "∅" Unicode : \u2205 |
| Increment | `6` | "∆" Unicode : \u2206 |
| Nabla | `7` | "∇" Unicode : \u2207 |
| ElementOf | `8` | "∈" Unicode : \u2208 |
| NotAnElementOf | `9` | "∉" Unicode : \u2209 |
| SmallElementOf | `10` | "∊" Unicode:\u220a |
| Contain | `11` | "∋" Unicode:\u220b |
| NotContain | `12` | "∌" Unicode:\u220c |
| SmallContain | `13` | "∍" Unicode:\u220d |
| EndOfProof | `14` | "∎" Unicode:\u220e |
| NaryProduct | `15` | "∏" Unicode:\u220f |
| NaryCoproduct | `16` | "∐" Unicode:\u2210 |
| NarySummation | `17` | "∑" Unicode:\u2211 |
| LogicalAnd | `18` | "∧" Unicode:\u2227 |
| LogicalOr | `19` | "∨" Unicode:\u2228 |
| Intersection | `20` | "∩" Unicode:\u2229 |
| Union | `21` | "∪" Unicode:\u222a |
| Integral | `22` | "∫" Unicode:\u222b |
| DoubleIntegral | `23` | "∬" Unicode:\u222c |
| TripleIntegral | `24` | "∭" Unicode:\u222d |
| ContourIntegral | `25` | "∮" Unicode:\u222e |
| SurfaceIntegral | `26` | "∯" Unicode:\u222f |
| VolumeIntegral | `27` | "∰" Unicode:\u2230 |
| Clockwise | `28` | "∱" Unicode:\u2231 |
| ClockwiseContourIntegral | `29` | "∲" Unicode:\u2232 |
| AnticlockwiseContourIntegral | `30` | "∳" Unicode:\u2233 |
| NaryLogicalAnd | `31` | "⋀" Unicode:\u22c0 |
| NaryLogicalOr | `32` | "⋁" Unicode:\u22c1 |
| NaryIntersection | `33` | "⋂" Unicode:\u22c2 |
| NaryUnion | `34` | "⋃" Unicode:\u22c3 |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationMathematicalOperatorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte pour insérer des opérateurs mathématiques
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 0, 0);
            textBox.Text = "Mathematical Operators Demo:\n";

            // Démontrer diverses valeurs de EquationMathematicalOperatorType
            textBox.Text += $"ForAll: {(char)0x2200}\n";
            textBox.Text += $"Complement: {(char)0x2201}\n";
            textBox.Text += $"PartialDifferential: {(char)0x2202}\n";
            textBox.Text += $"Exists: {(char)0x2203}\n";
            textBox.Text += $"NarySummation: {(char)0x2211}\n";
            textBox.Text += $"LogicalAnd: {(char)0x2227}\n";
            textBox.Text += $"LogicalOr: {(char)0x2228}\n";
            textBox.Text += $"Integral: {(char)0x222B}\n";
            textBox.Text += $"DoubleIntegral: {(char)0x222C}\n";
            textBox.Text += $"NaryLogicalAnd: {(char)0x22C0}\n";

            // Utiliser directement les valeurs de l'énumération
            EquationMathematicalOperatorType operatorType = EquationMathematicalOperatorType.NarySummation;
            textBox.Text += $"\nSelected operator via enum: {operatorType} ({(char)0x2211})";

            // Enregistrer le résultat
            workbook.Save("EquationMathematicalOperatorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


