---
title: "Classe ConnectionParameter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExternalConnections.ConnectionParameter. Specifica le proprietà di tutti i parametri utilizzati con connessioni dati esterne. I parametri sono validi per ODBC e query web"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Specifica le proprietà di tutti i parametri utilizzati con connessioni dati esterne. I parametri sono validi per ODBC e query web.

```csharp
public class ConnectionParameter
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Il nome del parametro. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se vero, i dati esterni vengono aggiornati usando il nuovo valore del parametro ogni volta che si verifica una modifica. Se falso, i dati esterni vengono aggiornati solo quando richiesto dall'utente, o quando qualche altro evento attiva l'aggiornamento (ad es., cartella di lavoro aperta). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | Tipo di dati SQL del parametro. Valido solo per le origini ODBC. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Tipo di parametro utilizzato. Se parameterType=value, allora il valore da boolean, double, integer o string verrà usato. In questo caso, ci si aspetta che venga specificato solo uno tra {boolean, double, integer, or string}. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. Usato solo quando parameterType è valore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            
            try
            {
                // Crea un parametro di connessione usando la reflection poiché il costruttore non è pubblico
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Imposta le proprietà di base
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Visualizza le informazioni del parametro
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


