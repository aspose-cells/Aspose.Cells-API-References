---
title: "Worksheet.SetVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Legt die Sichtbarkeitsoptionen fest"
type: docs
url: /de/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Legt die sichtbaren Optionen fest.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isVisible | Boolean | Ob das Arbeitsblatt sichtbar ist |
| ignoreError | Boolean | Ob ein Fehler ignoriert werden soll, wenn diese Option nicht gültig ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Einige Arbeitsblätter hinzufügen
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Sichtbarkeit von Arbeitsblättern festlegen
            // Erster Parameter: isVisible - false, um das Blatt zu verbergen
            // Zweiter Parameter: ignoreError - true, um den Fehler zu ignorieren, wenn das Blatt nicht ausgeblendet werden kann
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


