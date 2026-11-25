---
title: "ExternalConnection.CredentialsMethodType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. Specifica il metodo di autenticazione da utilizzare quando si stabilisce o si ristabilisce la connessione"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Specifica il metodo di autenticazione da utilizzare quando si stabilisce (o si ristabilisce) la connessione.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Aggiungi un foglio di lavoro e crea una tabella pivot per stabilire una connessione esterna
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Crea una tabella pivot che avrà una connessione esterna
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Ottieni la connessione esterna dalla tabella pivot
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Visualizza il valore corrente di CredentialsMethodType
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Dimostra l'impostazione della proprietà (poiché è leggibile e scrivibile)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Imposta a un altro valore per dimostrare
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Salva la cartella di lavoro con le impostazioni di connessione modificate
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


