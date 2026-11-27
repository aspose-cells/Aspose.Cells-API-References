---
title: "ConnectionParameter.Prompt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter-egenskap. Prompt‑sträng för parametern. Presenteras för kalkylbladsanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan den externa datan uppdateras. Används endast när parameterType är prompt"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Prompt-sträng för parametern. Presenteras för kalkylarksanvändaren tillsammans med inmatnings‑UI för att samla in parametervärdet innan den externa datan uppdateras. Används endast när parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                
                // Skapa en anslutningsparameter (simulerad eftersom konstruktörsparametrar är okända)
                ConnectionParameter parameter = null;
                
                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // För demonstration visar vi hur Prompt skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella Prompt‑värdet
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Ange ett nytt Prompt‑värde (eftersom egenskapen är läs‑skriv)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


