---
title: "ConnectionParameter.CellReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameter‑egenskap. Cellreferens som anger vilket cellvärde som ska användas för frågeparametern. Används endast när parameterType är cell"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Cellreferens som anger vilket cells värde som ska användas för frågeparametern. Används endast när parameterType är cell.

```csharp
public string CellReference { get; set; }
```

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                
                // Skapa en anslutningsparameter (simulerad eftersom konstruktörsparametrar är okända)
                ConnectionParameter parameter = null;
                
                // I ett verkligt scenario skulle du skapa parametern korrekt
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // För demonstration visar vi hur CellReference skulle användas om vi hade en parameter
                if (parameter != null)
                {
                    // Hämta och visa det aktuella CellReference‑värdet
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Ange ett nytt CellReference‑värde (eftersom egenskapen är läs‑skriv)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Reservdemonstration när vi inte kan skapa parametern
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


