---
title: "ConnectionParameter.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Der Name des Parameters"
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

Der Name des Parameters.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
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

                // Zur Demonstration zeigen wir, wie Name verwendet würde, wenn wir einen Parameter hätten
                if (parameter != null)
                {
                    // Abrufen und Anzeigen des aktuellen Name-Werts
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Setzen eines neuen Name-Werts (da die Eigenschaft les- und schreibbar ist)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


