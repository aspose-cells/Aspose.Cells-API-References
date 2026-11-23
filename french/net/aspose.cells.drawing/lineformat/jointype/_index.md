---
title: "LineFormat.JoinType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LineFormat. Spécifie le type de jointure de ligne"
type: docs
url: /fr/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Spécifie le type de jointure de ligne.

```csharp
public LineJoinType JoinType { get; set; }
```

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme de ligne
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Définir le type de jointure de ligne sur Arrondi
            line.Line.JoinType = LineJoinType.Round;

            // Enregistrez le classeur
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


