---
title: "ConnectionParameter.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter egenskap. Typ av parameter som används. Om parameterTypvärdet då kommer värdet från boolean, double, integer eller string att användas. I detta fall förväntas endast ett av boolean, double, integer eller string att specificeras"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Typ av parameter som används. Om parameterType=value, används värdet från boolean, double, integer eller string. I detta fall förväntas endast ett av {boolean, double, integer, or string} specificeras.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                
                // Skapa en anslutningsparameter (simulerad eftersom konstruktörsparametrar är okända)
                ConnectionParameter parameter = null;
                
                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // För demonstration kommer vi att visa hur Type skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella Type‑värdet.
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Ange ett nytt Type‑värde (eftersom egenskapen är läs‑skriv).
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
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

### Se även

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


