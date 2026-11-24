---
title: "Enum EquationDelimiterShapeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType enum. Dies gibt die Form der Trennzeichen im Trennzeichenobjekt an."
type: docs
url: /de/net/aspose.cells.drawing.equations/equationdelimitershapetype/
---
## EquationDelimiterShapeType enumeration

Dies gibt die Form der Trennzeichen im Trennzeichenobjekt an.

```csharp
public enum EquationDelimiterShapeType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Centered | `0` | Der Trenner ist um die gesamte Höhe seines Inhalts zentriert. |
| Match | `1` | Der Trenner wird so angepasst, dass er exakt die Höhe ihres Inhalts entspricht. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class EquationsClassEquationDelimiterShapeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gleichungsform hinzufügen
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // Gleichungsknoten abrufen
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // Trennzeichen-Knoten mit Match-Formtyp erstellen
            DelimiterEquationNode delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "{";
            delimiterNode.EndChar = "}";
            
            // Inhalt innerhalb des Trennzeichens hinzufügen
            EquationNode baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";
            
            // Speichere die Arbeitsmappe
            workbook.Save("EquationDelimiterShapeTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


