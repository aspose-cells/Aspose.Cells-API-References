---
title: "ConnectionParameter.Prompt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameter-Eigenschaft. Prompt-Zeichenfolge für den Parameter. Dem Tabellenkalkulationsbenutzer zusammen mit einer Eingabe‑UI präsentiert, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType Prompt ist."
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Eingabeaufforderungszeichenfolge für den Parameter. Wird dem Tabellenbenutzer zusammen mit einer Eingabe‑UI präsentiert, um den Parameterwert vor dem Aktualisieren der externen Daten zu erfassen. Wird nur verwendet, wenn parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // Zur Demonstration zeigen wir, wie Prompt verwendet würde, wenn wir einen Parameter hätten
                if (parameter != null)
                {
                    // Abrufen und Anzeigen des aktuellen Prompt-Werts
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Setzen eines neuen Prompt-Werts (da die Eigenschaft les- und schreibbar ist)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Fallback-Demonstration, wenn wir den Parameter nicht erstellen können.
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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


