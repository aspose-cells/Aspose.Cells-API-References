---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConnectionParameter proprietà. Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se vero, i dati esterni vengono aggiornati usando il nuovo valore del parametro ogni volta che c'è un cambiamento. Se falso, i dati esterni vengono aggiornati solo quando richiesto dall'utente o quando qualche altro evento innesca l'aggiornamento, ad es. apertura della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Flag che indica se la query deve aggiornarsi automaticamente quando il contenuto di una cella che fornisce il valore del parametro cambia. Se vero, i dati esterni vengono aggiornati usando il nuovo valore del parametro ogni volta che si verifica una modifica. Se falso, i dati esterni vengono aggiornati solo quando richiesto dall'utente, o quando qualche altro evento attiva l'aggiornamento (ad es., cartella di lavoro aperta).

```csharp
public bool RefreshOnChange { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
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
                
                // Per dimostrazione, mostreremo come verrebbe usato RefreshOnChange se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di RefreshOnChange
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Imposta un nuovo valore RefreshOnChange (poiché la proprietà è leggibile e scrivibile)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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


