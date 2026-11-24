---
title: "AutoFilter.SetRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird"
type: docs
url: /de/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Legt den Bereich fest, auf den der angegebene AutoFilter angewendet wird.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| startColumn | Int32 | Startspaltenindex. |
| endColumn | Int32 | Endspalten-Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Auto-Filter-Bereich festlegen (ersteZeile, ersteSpalte, Gesamtzeilen)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Filter anwenden
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Filter aktualisieren
            sheet.AutoFilter.Refresh();

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


