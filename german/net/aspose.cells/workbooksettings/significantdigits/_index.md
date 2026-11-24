---
title: "WorkbookSettings.SignificantDigits"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt die Anzahl signifikanter Stellen zurück und legt sie fest. Der Standardwert ist SignificantDigits"
type: docs
url: /de/net/aspose.cells/workbooksettings/significantdigits/
---
## WorkbookSettings.SignificantDigits property

Gibt die Anzahl signifikanter Stellen zurück und legt sie fest. Der Standardwert ist [`SignificantDigits`](../../cellshelper/significantdigits/).

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int SignificantDigits { get; set; }
```

### Hinweise

Nur noch 15 oder 17 möglich. HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte [`SignificantDigitsType`](../significantdigitstype/). Diese Eigenschaft wird 12 Monate später, seit Juni 2025, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu, um signifikante Stellen zu demonstrieren
            sheet.Cells["A1"].PutValue(123.4567890123456789);
            sheet.Cells["A2"].PutValue(0.000000000123456789);

            // Auf Arbeitsmappeneinstellungen zugreifen
            WorkbookSettings settings = workbook.Settings;

            // Setzen Sie signifikante Stellen auf 15 (maximale Genauigkeit für double)
            settings.SignificantDigits = 15;

            // Speichern Sie die Arbeitsmappe, um die Wirkung signifikanter Stellen zu zeigen
            workbook.Save("SignificantDigitsDemo.xlsx");

            Console.WriteLine("Workbook saved with SignificantDigits set to 15.");
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


