---
title: "CalculationOptions.CharacterEncoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Gibt die für das Codieren/Dekodieren von Zeichen bei der Berechnung von Formeln verwendete Kodierung an. Für Funktionen wie CHAR CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standardzeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die richtige Kodierung für diese Funktionen angeben, um das erwartete Ergebnis zu erhalten."
type: docs
url: /de/net/aspose.cells/calculationoptions/characterencoding/
---
## CalculationOptions.CharacterEncoding property

Gibt die beim Berechnen von Formeln zu verwendende Kodierung für das Codieren/Dekodieren von Zeichen an. Für Funktionen wie CHAR, CODE hängt das berechnete Ergebnis von den Regionseinstellungen und dem Standard‑Zeichensatz der Umgebung ab. Mit dieser Eigenschaft kann der Benutzer die geeignete Kodierung für diese Funktionen festlegen, um das erwartete Ergebnis zu erhalten.

```csharp
public Encoding CharacterEncoding { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCharacterEncodingDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            wb.Settings.Region = CountryCode.Japan;
            
            CalculationOptions copts = new CalculationOptions();
            copts.CharacterEncoding = Encoding.GetEncoding("iso-2022-jp");
            
            string formula = "=TRIM(1)";
            string result = (string)sheet.CalculateFormula(formula, copts);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


