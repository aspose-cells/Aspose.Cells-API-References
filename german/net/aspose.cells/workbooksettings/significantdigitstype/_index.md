---
title: "WorkbookSettings.SignificantDigitsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest und setzt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Standardwert ist SignificantDigitsType"
type: docs
url: /de/net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Liest und setzt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte in dieser Arbeitsmappe. Standardwert ist [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greift auf die WorkbookSettings zu.
            WorkbookSettings settings = workbook.Settings;

            // Zeige den aktuellen SignificantDigitsType-Wert an
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Demonstrieren Sie das Festlegen verschiedener SignificantDigitsType‑Werte
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Fügen Sie einige numerische Daten hinzu, um die Wirkung zu demonstrieren
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Speichere die Arbeitsmappe
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### Siehe auch

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


