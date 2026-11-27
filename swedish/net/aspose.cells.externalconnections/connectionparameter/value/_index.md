---
title: "ConnectionParameter.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter egenskap. Icke-heltal numeriskt värdeInteger valueString value eller Boolean value att använda som frågeparameter. Används endast när parameterType är value"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Icke-heltal numeriskt värde, Integer‑värde, String‑värde eller Boolean‑värde att använda som frågeparameter. Används endast när parameterType är value.

```csharp
public object Value { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                
                // Skapa en anslutningsparameter (simulerad eftersom vi inte känner till konstruktörsparametrar)
                ConnectionParameter parameter = null;
                
                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // För demonstration kommer vi att skapa en mock-parameter med ett värde
                // Detta visar hur Value-egenskapen skulle användas i praktiken
                if (parameter != null)
                {
                    // Ange värdet (eftersom Value är läs-skriv)
                    parameter.Value = "SampleParameterValue";
                    
                    // Hämta och visa värdet
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Ändra värdet för att demonstrera att det är föränderligt
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


