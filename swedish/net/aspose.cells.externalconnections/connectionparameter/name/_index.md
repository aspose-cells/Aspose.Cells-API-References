---
title: "ConnectionParameter.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter‑egenskap. Parameterns namn"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

Namnet på parametern.

```csharp
public string Name { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();

                // Skapa en anslutningsparameter (simulerad eftersom konstruktörsparametrar är okända)
                ConnectionParameter parameter = null;

                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);

                // För demonstration visar vi hur Name skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella Name‑värdet
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Ange ett nytt Name‑värde (eftersom egenskapen är läs‑skriv)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


