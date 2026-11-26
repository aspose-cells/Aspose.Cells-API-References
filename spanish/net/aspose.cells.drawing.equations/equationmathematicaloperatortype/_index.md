---
title: "Enum EquationMathematicalOperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.Equations.EquationMathematicalOperatorType enum. Tipo de Operadores Matemáticos"
type: docs
url: /es/net/aspose.cells.drawing.equations/equationmathematicaloperatortype/
---
## EquationMathematicalOperatorType enumeration

Tipo de operadores matemáticos

```csharp
public enum EquationMathematicalOperatorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Unknown | `-1` | Usar tipo desconocido cuando no se encuentre en el tipo existente. |
| ForAll | `0` | "∀" Unicode:\u2200 |
| Complement | `1` | "∁" Unicode:\u2201 |
| PartialDifferential | `2` | "∂" Unicode:\u2202 |
| Exists | `3` | "∃" Unicode:\u2203 |
| NotExists | `4` | "∄" Unicode:\u2204 |
| EmptySet | `5` | "∅" Unicode:\u2205 |
| Increment | `6` | "∆" Unicode:\u2206 |
| Nabla | `7` | "∇" Unicode:\u2207 |
| ElementOf | `8` | "∈" Unicode:\u2208 |
| NotAnElementOf | `9` | "∉" Unicode:\u2209 |
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

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto para insertar operadores matemáticos
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 0, 0);
            textBox.Text = "Mathematical Operators Demo:\n";

            // Demostrar varios valores de EquationMathematicalOperatorType
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

            // Usar los valores del enum directamente
            EquationMathematicalOperatorType operatorType = EquationMathematicalOperatorType.NarySummation;
            textBox.Text += $"\nSelected operator via enum: {operatorType} ({(char)0x2211})";

            // Guardar el resultado
            workbook.Save("EquationMathematicalOperatorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


