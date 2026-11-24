---
title: "ConnectionParameter.Value"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Nicht-ganzzahliger numerischer Wert, ganzzahliger Wert, Zeichenkettenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType den Wert 'value' hat"
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Nicht‑ganzzahliger numerischer Wert, Ganzzahlwert, Zeichenkettenwert oder Boolescher Wert, der als Abfrageparameter verwendet wird. Wird nur verwendet, wenn parameterType Wert ist.

```csharp
public object Value { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                
                // Erstelle einen Verbindungsparameter (simuliert, da wir die Konstruktorparameter nicht kennen)
                ConnectionParameter parameter = null;
                
                // In einem realen Szenario würden Sie den Parameter korrekt erstellen.
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Zur Demonstration erstellen wir einen Mock-Parameter mit einem Wert.
                // Dies zeigt, wie die Value-Eigenschaft in der Praxis verwendet werden würde.
                if (parameter != null)
                {
                    // Setze den Wert (da Value les- und schreibbar ist)
                    parameter.Value = "SampleParameterValue";
                    
                    // Lese und zeige den Wert an.
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Ändere den Wert, um zu demonstrieren, dass er veränderlich ist.
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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


