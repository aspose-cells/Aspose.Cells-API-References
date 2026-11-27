---
title: "ExternalConnection.SecondCommand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger en andra kommandotextsträng som sparas när PivotTable serversidiga sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command eftersom ingen WHERE-klausul finns i den förstnämnda. Baserat på dessa två kommandon, Command och ServerCommand, kan UI-parametrar fyllas i och parametriserade frågor konstrueras"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Anger en andra kommandotextsträng som bevaras när PivotTable-serverbaserade sidfält används. För ODBC-anslutningar är serverCommand vanligtvis en bredare fråga än command (ingen WHERE-klausul finns i den förra). Baserat på dessa två kommandon (Command och ServerCommand) kan parameter‑UI fyllas i och parametriserade frågor konstrueras

```csharp
public virtual string SecondCommand { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella SecondCommand-värdet (läsoperation)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Ange ett nytt SecondCommand-värde (eftersom den är läs-skriv)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Rensa SecondCommand för att demonstrera att sätta en tom sträng
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


