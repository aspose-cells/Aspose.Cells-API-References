---
title: "ExternalConnection.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Hämtar eller anger den externa anslutningens DataSource‑typ"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Hämtar eller anger den externa anslutningens DataSource‑typ.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället ExternalConnection.SourceType property. Den här egenskapen kommer att tas bort 12 månader senare sedan oktober 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella Type‑värdet (läsoperation)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Ange ett nytt Type‑värde (eftersom det är läs‑/skrivbart)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Cykla igenom möjliga värden för att demonstrera inställningsmöjligheten
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


