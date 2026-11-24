---
title: "Enum VisibilityType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.VisibilityType enum. Stellt die Zustände für die Blatt‑Sichtbarkeit dar"
type: docs
url: /de/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Stellt die Zustände für die Sichtbarkeit des Blatts dar.

```csharp
public enum VisibilityType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Visible | `0` | Zeigt an, dass das Blatt sichtbar ist. |
| Hidden | `1` | Zeigt an, dass das Blatt ausgeblendet ist, aber vom Benutzer über die Benutzeroberfläche angezeigt werden kann. |
| VeryHidden | `2` | Zeigt an, dass das Blatt ausgeblendet ist und in der Benutzeroberfläche (UI) nicht angezeigt werden kann. Dieser Zustand ist nur programmgesteuert verfügbar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie den Namen des Arbeitsblatts
            worksheet.Name = "DemoSheet";

            // Setzen Sie die Sichtbarkeit des Arbeitsblatts auf Ausgeblendet
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Speichere die Arbeitsmappe
            workbook.Save("VisibilityTypeExample.xlsx");

            // Ausgabe, um anzuzeigen, dass der Vorgang abgeschlossen ist
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


