---
title: "Schnittstelle IWarningCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IWarningCallback Schnittstelle. Callback‑Schnittstelle für Warnungen"
type: docs
url: /de/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Callback‑Schnittstelle für Warnungen.

```csharp
public interface IWarningCallback
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Unser Callback muss nur die Methode "Warning" implementieren. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Implementierung der Warning‑Methode aus der IWarningCallback‑Schnittstelle
        public void Warning(WarningInfo warningInfo)
        {
            // Zeigt die Warnmeldung an
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Setzt den Warn‑Callback
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Lädt eine Arbeitsmappe mit potenziellen Warnungen
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


