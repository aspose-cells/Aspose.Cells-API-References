---
title: "ExternalConnection.SavePassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExternalConnection. True se la password deve essere salvata come parte della stringa di connessione, altrimenti False"
type: docs
url: /it/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

True se la password deve essere salvata come parte della stringa di connessione; altrimenti, False.

```csharp
public bool SavePassword { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            try
            {
                // Accedi alla prima connessione esterna (supponendo che ne esista una)
                ExternalConnection connection = workbook.DataConnections[0];

                // Visualizza il valore corrente di SavePassword
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Dimostra l'impostazione della proprietà (poiché è leggibile e scrivibile)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Attiva/disattiva il valore per dimostrare la capacità di impostazione
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Salva la cartella di lavoro con le impostazioni di connessione modificate
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

### Vedi anche

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


