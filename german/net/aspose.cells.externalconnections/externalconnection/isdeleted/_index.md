---
title: "ExternalConnection.IsDeleted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalConnection property. Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde, sonst false"
type: docs
url: /de/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Gibt an, ob die zugehörige Arbeitsmappenverbindung gelöscht wurde. true, wenn die Verbindung gelöscht wurde; andernfalls false.

```csharp
public bool IsDeleted { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die erste externe Verbindung zu (sofern eine vorhanden ist)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Zeigen Sie den anfänglichen IsDeleted-Wert an
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Schalten Sie den IsDeleted-Wert um (da er les- und schreibbar ist)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Speichern Sie die Arbeitsmappe mit den geänderten Verbindungseinstellungen
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

### Siehe auch

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


