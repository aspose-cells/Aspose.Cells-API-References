---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. Wenn true, werden die externen Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn false, werden die externen Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst, z. B. beim Öffnen der Arbeitsmappe."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Flag, das angibt, ob die Abfrage automatisch aktualisiert werden soll, wenn sich der Inhalt einer Zelle, die den Parameterwert liefert, ändert. Wenn wahr, werden die externen Daten bei jeder Änderung mit dem neuen Parameterwert aktualisiert. Wenn falsch, werden die externen Daten nur aktualisiert, wenn der Benutzer dies anfordert oder ein anderes Ereignis die Aktualisierung auslöst (z. B. beim Öffnen der Arbeitsmappe).

```csharp
public bool RefreshOnChange { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                
                // Erstelle einen Verbindungsparameter (simuliert, da die Konstruktorparameter unbekannt sind)
                ConnectionParameter parameter = null;
                
                // In einem realen Szenario würden Sie den Parameter korrekt erstellen.
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Zur Demonstration zeigen wir, wie RefreshOnChange verwendet würde, wenn wir einen Parameter hätten
                if (parameter != null)
                {
                    // Abrufen und Anzeigen des aktuellen RefreshOnChange-Werts
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Setzen eines neuen RefreshOnChange-Werts (da die Eigenschaft les- und schreibbar ist)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


