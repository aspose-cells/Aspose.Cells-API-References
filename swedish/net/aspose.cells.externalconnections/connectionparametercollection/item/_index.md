---
title: "ConnectionParameterCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConnectionParameterCollection‑egenskap. Hämtar ConnectionParameter‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Hämtar [`ConnectionParameter`](../../connectionparameter/) elementet på det angivna indexet.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Hämta den första externa anslutningen
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Hämta parameterns samling
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Kontrollera om det finns några parametrar innan åtkomst
                if (parameters.Count > 0)
                {
                    // Demonstrera läsning av Item-egenskapen
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Hämtar elementet [`ConnectionParameter`](../../connectionparameter/) med det angivna namnet.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| connParamName | namn på anslutningsparameter |

### Returvärde

Elementet med det angivna namnet.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Hämta den första externa anslutningen
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Hämta parameterns samling
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Kontrollera om det finns befintliga parametrar för att demonstrera Item-egenskapen
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Hämta namnet på den första parametern att använda för demonstration
                string firstParamName = parameters[0].Name;
                
                // Demonstrera läsning av Item-egenskapen med namn
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Spara arbetsboken
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

### Se även

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


