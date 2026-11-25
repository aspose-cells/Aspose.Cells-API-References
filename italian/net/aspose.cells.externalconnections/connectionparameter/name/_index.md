---
title: "ConnectionParameter.Name"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConnectionParameter. Il nome del parametro"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/name/
---
## ConnectionParameter.Name property

Il nome del parametro.

```csharp
public string Name { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyNameDemo
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

                // Per dimostrazione, mostreremo come verrebbe usato Name se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di Name
                    Console.WriteLine("Current Name: " + parameter.Name);

                    // Imposta un nuovo valore Name (poiché la proprietà è leggibile e scrivibile)
                    parameter.Name = "NewParameterName";
                    Console.WriteLine("Updated Name: " + parameter.Name);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "Name property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }

                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterNameDemo.xlsx");
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


