---
title: "ConnectionParameterCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConnectionParameterCollection-Eigenschaft. Gibt das ConnectionParameter-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Gibt das [`ConnectionParameter`](../../connectionparameter/) Element am angegebenen Index zurück.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erhalte die erste externe Verbindung
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Erhalte die Parametersammlung
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Prüfe, ob Parameter vorhanden sind, bevor zugegriffen wird
                if (parameters.Count > 0)
                {
                    // Demonstriere das Lesen der Item-Eigenschaft
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Gibt das [`ConnectionParameter`](../../connectionparameter/) Element mit dem angegebenen Namen zurück.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| connParamName | Name des Verbindungsparameters |

### Rückgabewert

Das Element mit dem angegebenen Namen.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erhalte die erste externe Verbindung
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Erhalte die Parametersammlung
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Überprüfen, ob vorhandene Parameter existieren, um die Item‑Eigenschaft zu demonstrieren
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Den Namen des ersten Parameters für die Demonstration erhalten
                string firstParamName = parameters[0].Name;
                
                // Demonstriere das Auslesen der Item‑Eigenschaft per Name
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


