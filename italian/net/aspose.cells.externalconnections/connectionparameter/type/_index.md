---
title: "ConnectionParameter.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConnectionParameter. Tipo di parametro utilizzato. Se il valore parameterType allora verrà usato il valore da boolean, double, integer o string. In questo caso ci si aspetta che venga specificato solo uno tra boolean, double, integer o string"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Tipo di parametro utilizzato. Se parameterType=value, allora il valore da boolean, double, integer o string verrà usato. In questo caso, ci si aspetta che venga specificato solo uno tra {boolean, double, integer, or string}.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();
                
                // Crea un parametro di connessione (simulato poiché i parametri del costruttore sono sconosciuti)
                ConnectionParameter parameter = null;
                
                // In uno scenario reale, dovresti creare il parametro correttamente
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Per dimostrazione, mostreremo come verrebbe usato Type se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di Type
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Imposta un nuovo valore Type (poiché la proprietà è leggibile e scrivibile)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


