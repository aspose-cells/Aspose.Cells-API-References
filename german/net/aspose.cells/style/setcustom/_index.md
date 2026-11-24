---
title: "Style.SetCustom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Legt die benutzerdefinierte Zahlenformatzeichenfolge einer Zelle fest."
type: docs
url: /de/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Setzt die Custom-Zahlenformatzeichenfolge einer Zelle.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| benutzerdefiniert | String | Benutzerdefinierte Zahlenformatzeichenfolge, sollte ein InvariantCulture-Muster sein. |
| builtinPreference | Boolean | Wenn die angegebene benutzerdefinierte Zahlenformatzeichenfolge mit einem der integrierten Zahlenformate übereinstimmt, die den aktuellen regionalen Einstellungen entsprechen, wird das Zahlenformat als integriert statt benutzerdefiniert festgelegt. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodSetCustomWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Style style = wb.CreateStyle();
            
            string customFormat1 = "_(\"$\"* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat1, true);
            Console.WriteLine("Custom format 1 applied. Style number: " + style.Number);

            string customFormat2 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* \"-\"??_);_(@_)";
            style.SetCustom(customFormat2, true);
            Console.WriteLine("Custom format 2 applied. Style number: " + style.Number);

            string customFormat3 = "_($* #,##0.00_);_(\"$\"* (#,##0.00);_(\"$\"* -??_);_(@_)";
            style.SetCustom(customFormat3, true);
            Console.WriteLine("Custom format 3 applied. Style number: " + style.Number);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


