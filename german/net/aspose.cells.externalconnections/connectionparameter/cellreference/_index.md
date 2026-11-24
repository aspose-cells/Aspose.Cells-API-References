---
title: "ConnectionParameter.CellReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Zellreferenz, die angibt, welchen Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType cell ist."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Zellreferenz, die angibt, welcher Zellenwert für den Abfrageparameter verwendet werden soll. Wird nur verwendet, wenn parameterType Zelle ist.

```csharp
public string CellReference { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // Zur Demonstration zeigen wir, wie CellReference verwendet würde, wenn wir einen Parameter hätten
                if (parameter != null)
                {
                    // Abrufen und Anzeigen des aktuellen CellReference-Werts
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Setzen eines neuen CellReference-Werts (da die Eigenschaft les- und schreibbar ist)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


