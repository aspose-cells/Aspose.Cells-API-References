---
title: "Row.CopySettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Methode. Kopiere Einstellungen der Zeile wie Stil, Höhe, Sichtbarkeit ...usw"
type: docs
url: /de/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Kopiert Einstellungen der Zeile, wie Stil, Höhe, Sichtbarkeit, ...usw.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | Row | die Quellzeile, deren Einstellungen auf diese kopiert werden |
| checkStyle | Boolean | ob Stil geprüft und gesammelt wird. Wirkt nur und ist erforderlich, wenn zwei Zeilenobjekte zu unterschiedlichen Arbeitsmappen gehören und die Stile der beiden Arbeitsmappen unterschiedlich sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle und formatiere die Quellzeile
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Erstelle Zielzeile
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Demonstriere CopySettings mit copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // Überprüfe, ob die Einstellungen kopiert wurden
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


