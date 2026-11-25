---
title: "WebQueryConnection.ClassType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "WebQueryConnection proprietà. Ottiene il tipo di questo oggetto ExternalConnection"
type: docs
url: /it/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

Ottiene il tipo di questo [`ExternalConnection`](../../externalconnection/) oggetto.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi a una connessione di query web esistente o creane una tramite un'adeguata inizializzazione
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Visualizza il valore di ClassType (proprietà di sola lettura)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Verifica il valore enum previsto per la query web
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Salva la cartella di lavoro
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


