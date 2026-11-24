---
title: "Row.IsHeightMatched"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung der Arbeitsmappe übereinstimmt. Der Wert true dieser Eigenschaft bedeutet zudem, dass die Zeilenhöhe automatisch ist, ohne dass ein benutzerdefinierter Höhenwert gesetzt wurde."
type: docs
url: /de/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Gibt an, ob die Zeilenhöhe mit der aktuellen Standardschriftart-Einstellung des Arbeitsbuchs übereinstimmt. Der Wert true dieser Eigenschaft bedeutet außerdem, dass die Zeilenhöhe "automatisch" ist, ohne dass ein benutzerdefinierter Höhenwert vom Benutzer festgelegt wurde.

```csharp
public bool IsHeightMatched { get; set; }
```

### Hinweise

Wenn diese Eigenschaft true ist und sich der Inhalt dieser Zeile ändert, muss die Zeilenhöhe in der Regel neu berechnet werden (zum Beispiel durch [`AutoFitRows`](../../worksheet/autofitrows/)), um dasselbe Ergebnis zu erhalten, das in MS Excel angezeigt wird, wenn du die Arbeitsmappe dort öffnest.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze Beispieldaten und Formatierung, um die Übereinstimmung der Zeilenhöhe zu demonstrieren
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Wende Zeilenumbruch an, um die Höhenanpassung zu erzwingen
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Auto-fit die Zeile, um die Höhe des Inhalts anzupassen
            worksheet.AutoFitRow(0);
            
            // Überprüfe, ob die Zeilenhöhe mit ihrem Inhalt übereinstimmt
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Siehe auch

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


