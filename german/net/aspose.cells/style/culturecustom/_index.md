---
title: "Style.CultureCustom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die kulturspezifische Musterzeichenfolge für das Zahlenformat zurück und setzt sie. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben."
type: docs
url: /de/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Liest und setzt die kulturspezifische Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben.

```csharp
public string CultureCustom { get; set; }
```

### Hinweise

Bei eingebauten Zahlenformaten sind sowohl der Musterinhalt (z. B. ein eingebautes Datumsformat ist für einige Gebietsschemas "m/d/y", für andere wird es zu "d/m/y") als auch der Formatbezeichner (z. B. verwenden einige Gebietsschemas ein anderes Zeichen als 'y', um den Jahresanteil im Datumsformat darzustellen) kulturbabhängig; Bei vom Benutzer angegebenen benutzerdefinierten Formaten werden nur die Formatbezeichner gemäß der Kultur geändert, andere Teile des Formatmusters bleiben unverändert.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und setzen Sie die ungarische Kultur.
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Holen Sie die erste Zelle und ihren Stil.
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Setzen Sie ein benutzerdefiniertes Format und demonstrieren Sie die CultureCustom-Konvertierung.
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Wenden Sie den Stil an und demonstrieren Sie kulturabhängige Formatierung
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Demonstrieren Sie die Formel mit kulturspezifischer Formatierung
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


