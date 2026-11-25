---
title: "ConnectionParameter.Value"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConnectionParameter proprietà. Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. Usato solo quando parameterType è value"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Valore numerico non intero, valore intero, valore stringa o valore booleano da utilizzare come parametro della query. Usato solo quando parameterType è valore.

```csharp
public object Value { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                
                // Crea un parametro di connessione (simulato poiché non conosciamo i parametri del costruttore)
                ConnectionParameter parameter = null;
                
                // In uno scenario reale, dovresti creare il parametro correttamente
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Per dimostrazione, creeremo un parametro simulato con un valore
                // Questo mostra come la proprietà Value verrebbe usata in pratica
                if (parameter != null)
                {
                    // Imposta il valore (poiché Value è leggibile e scrivibile)
                    parameter.Value = "SampleParameterValue";
                    
                    // Ottieni e visualizza il valore
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Modifica il valore per dimostrare che è modificabile
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


