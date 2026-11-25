---
title: "Style.SetCustom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Imposta la stringa di formato numerico Personalizzato di una cella"
type: docs
url: /it/net/aspose.cells/style/setcustom/
---
## Style.SetCustom method

Imposta la stringa di formato numerico personalizzato di una cella.

```csharp
public void SetCustom(string custom, bool builtinPreference)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| personalizzato | String | Stringa di formato numerico Personalizzato, dovrebbe essere un modello InvariantCulture. |
| builtinPreference | Booleano | Se la stringa di formato numerico Personalizzato fornita corrisponde a uno dei formati numerici integrati corrispondenti alle impostazioni regionali correnti, se impostare il formato numerico come integrato invece di Personalizzato. |

### Esempi

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

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


