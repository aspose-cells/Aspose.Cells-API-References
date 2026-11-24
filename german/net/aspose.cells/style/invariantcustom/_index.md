---
title: "Style.InvariantCustom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die kulturunabhängige Musterzeichenfolge für das Zahlenformat zurück. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Wenn das Zahlenformat eingebaut ist, wird die Musterzeichenfolge zurückgegeben, die dem eingebauten Zahlenformat entspricht."
type: docs
url: /de/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Liest die kulturlose Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben.

```csharp
public string InvariantCustom { get; }
```

### Hinweise

Bei eingebauten Zahlenformaten ist der zurückgegebene Musterinhalt weiterhin kulturabhängig, zum Beispiel gibt er für einige Gebietsschemas "m/d/y" zurück und für andere "d/m/y". Der Unterschied zu [`CultureCustom`](../culturecustom/) besteht darin (das ist auch das, was kulturunabhängig bedeutet): Die Formatbezeichner und Trennzeichen bleiben standardisiert, sodass '/' immer als Datums‑Trennzeichen verwendet wird und "y" immer den "Jahr"‑Teil darstellt, unabhängig davon, welches andere Sonderzeichen für das jeweilige Gebietsschema verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Datumsformat und Wert festlegen
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Ergebnisse ausgeben
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


