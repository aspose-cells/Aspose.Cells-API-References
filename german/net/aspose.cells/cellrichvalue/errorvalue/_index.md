---
title: "CellRichValue.ErrorValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellRichValue-Eigenschaft. Ruft den Fehlertyp des Zellenwerts ab"
type: docs
url: /de/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Liest den Fehlertypwert der Zelle.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen Spill-Fehler in Zelle A1 erzeugen
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Formeln berechnen, um den Spill-Fehler zu erzeugen
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Erwarteter Spill-Fehler
            }
            
            // Rich-Wert aus Zelle A1 abrufen
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Den Fehlertyp prüfen und anzeigen
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


