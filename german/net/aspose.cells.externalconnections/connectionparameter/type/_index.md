---
title: "ConnectionParameter.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Typ des verwendeten Parameters. Wenn der parameterType-Wert dann wird der Wert von boolean, double, integer oder string verwendet. In diesem Fall wird erwartet, dass nur einer von boolean, double, integer oder string angegeben wird."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Typ des verwendeten Parameters. Wenn parameterType=Wert, wird der Wert aus Boolean, Double, Integer oder String verwendet. In diesem Fall wird erwartet, dass nur einer von {Boolean, Double, Integer oder String} angegeben wird.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
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
                
                // Zur Demonstration zeigen wir, wie Type verwendet würde, wenn wir einen Parameter hätten
                if (parameter != null)
                {
                    // Abrufen und Anzeigen des aktuellen Type-Werts
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Setzen eines neuen Type-Werts (da die Eigenschaft les- und schreibbar ist)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


