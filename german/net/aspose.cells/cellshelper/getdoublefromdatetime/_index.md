---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Methode. Konvertiert das Datum und die Uhrzeit in einen Double-Wert"
type: docs
url: /de/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Konvertiert den DateTime-Wert in einen Double-Wert.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dateTime | DateTime | Das Datum und die Uhrzeit. |
| date1904 | Boolean | Datum-1904-System. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappeninstanz
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole das aktuelle Datum und die Uhrzeit
            DateTime now = DateTime.Now;
            
            // Konvertiere DateTime mit CellsHelper in einen Double
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // Setze den Wert in Zelle A1
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Formatiere die Zelle, um sie als Datum anzuzeigen
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


