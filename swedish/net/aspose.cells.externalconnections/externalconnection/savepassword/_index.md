---
title: "ExternalConnection.SavePassword"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Sant om lösenordet ska sparas som en del av anslutningssträngen, annars Falskt"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True om lösenordet ska sparas som en del av anslutningssträngen; annars False.

```csharp
public bool SavePassword { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visa det aktuella SavePassword-värdet
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Demonstrera att sätta egenskapen (eftersom den är läs-skriv)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Växla värdet för att demonstrera inställningsmöjlighet
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("SavePasswordDemo.xlsx");
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


