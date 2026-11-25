---
title: "Enum ConnectionParameterType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.ConnectionParameterType enum. Specifica il tipo di parametro della connessione esterna"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparametertype/
---
## ConnectionParameterType enumeration

Specifica il tipo di parametro della connessione esterna

```csharp
public enum ConnectionParameterType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Cell | `0` | Ottieni il valore del parametro da una cella ad ogni aggiornamento. |
| Prompt | `1` | Richiedi all'utente ad ogni aggiornamento un valore per il parametro. |
| Value | `2` | Usa un valore costante ad ogni aggiornamento per il valore del parametro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Dimostrare la creazione e l'uso dei valori enum ConnectionParameterType
                ConnectionParameterType cellParam = ConnectionParameterType.Cell;
                ConnectionParameterType promptParam = ConnectionParameterType.Prompt;
                ConnectionParameterType valueParam = ConnectionParameterType.Value;

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine("Connection Parameter Types:");
                Console.WriteLine($"Cell: {cellParam}");
                Console.WriteLine($"Prompt: {promptParam}");
                Console.WriteLine($"Value: {valueParam}");

                // Dimostrare l'uso in un'istruzione switch
                ConnectionParameterType testParam = ConnectionParameterType.Prompt;
                switch (testParam)
                {
                    case ConnectionParameterType.Cell:
                        Console.WriteLine("Parameter will get value from a cell");
                        break;
                    case ConnectionParameterType.Prompt:
                        Console.WriteLine("Parameter will prompt user for value");
                        break;
                    case ConnectionParameterType.Value:
                        Console.WriteLine("Parameter will use constant value");
                        break;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating ConnectionParameterType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


