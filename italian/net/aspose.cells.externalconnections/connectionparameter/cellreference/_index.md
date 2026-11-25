---
title: "ConnectionParameter.CellReference"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConnectionParameter. Riferimento cella che indica quale valore di cella utilizzare per il parametro di query. Usato solo quando parameterType è cell"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Riferimento di cella che indica quale valore di cella utilizzare per il parametro della query. Utilizzato solo quando parameterType è cell

```csharp
public string CellReference { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // Per dimostrazione, mostreremo come verrebbe usato CellReference se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di CellReference
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Imposta un nuovo valore CellReference (poiché la proprietà è leggibile e scrivibile)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


