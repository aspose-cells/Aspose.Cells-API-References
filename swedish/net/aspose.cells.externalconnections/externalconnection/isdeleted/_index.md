---
title: "ExternalConnection.IsDeleted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger om den associerade arbetsbokskopplingen har raderats. true om kopplingen har raderats annars false"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Indikerar om den associerade arbetsboksanslutningen har raderats. true om anslutningen har raderats; annars false.

```csharp
public bool IsDeleted { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det ursprungliga IsDeleted‑värdet
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Växla IsDeleted‑värdet (eftersom det är läs‑skriv)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("IsDeletedDemo.xlsx");
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


