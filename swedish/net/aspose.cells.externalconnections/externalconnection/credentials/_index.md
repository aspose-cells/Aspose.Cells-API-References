---
title: "ExternalConnection.Credentials"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalConnection egenskap. Anger autentiseringsmetoden som ska användas när anslutningen etableras eller återupprättas"
type: docs
url: /sv/net/aspose.cells.externalconnections/externalconnection/credentials/
---
## ExternalConnection.Credentials property

Anger autentiseringsmetoden som ska användas när anslutningen upprättas (eller återupprättas).

```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället ExternalConnection.CredentialsMethodType property. Den här egenskapen kommer att tas bort 12 månader senare sedan oktober 2017. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyCredentialsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till den första externa anslutningen (förutsatt att en sådan finns)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Visa det aktuella Credentials‑värdet
                Console.WriteLine("Initial Credentials value: " + connection.Credentials);
                
                // Ange ett nytt Credentials‑värde (eftersom det är läs‑/skrivbart)
                connection.Credentials = CredentialsMethodType.Integrated;
                Console.WriteLine("Updated Credentials value: " + connection.Credentials);
                
                // Cykla igenom möjliga värden
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    connection.Credentials = method;
                    Console.WriteLine($"Credentials set to: {method}");
                }
                
                // Spara arbetsboken med de ändrade anslutningsinställningarna
                workbook.Save("CredentialsDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


