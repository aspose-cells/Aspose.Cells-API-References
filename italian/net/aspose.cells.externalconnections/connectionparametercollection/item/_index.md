---
title: "ConnectionParameterCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConnectionParameterCollection proprietà. Ottiene l'elemento ConnectionParameter all'indice specificato"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Ottiene l'elemento [`ConnectionParameter`](../../connectionparameter/) all'indice specificato.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la prima connessione esterna
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Ottieni la collezione dei parametri
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Verifica se ci sono parametri prima di accedere
                if (parameters.Count > 0)
                {
                    // Dimostra la lettura della proprietà Item
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Ottiene l'elemento [`ConnectionParameter`](../../connectionparameter/) con il nome specificato.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| connParamName | nome del parametro di connessione |

### Valore di ritorno

L'elemento con il nome specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Ottieni la prima connessione esterna
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Ottieni la collezione dei parametri
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Verifica se esistono parametri per dimostrare la proprietà Item
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Ottieni il nome del primo parametro da utilizzare per la dimostrazione
                string firstParamName = parameters[0].Name;
                
                // Dimostra la lettura della proprietà Item per nome
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


