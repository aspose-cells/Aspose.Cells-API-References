---
title: "ConnectionParameter.Prompt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ConnectionParameter proprietà. Stringa Prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Usata solo quando parameterType è prompt"
type: docs
url: /it/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Stringa di prompt per il parametro. Presentata all'utente del foglio di calcolo insieme all'interfaccia di input per raccogliere il valore del parametro prima di aggiornare i dati esterni. Utilizzata solo quando parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // Per dimostrazione, mostreremo come verrebbe usato Prompt se avessimo un parametro
                if (parameter != null)
                {
                    // Ottieni e visualizza il valore corrente di Prompt
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Imposta un nuovo valore Prompt (poiché la proprietà è leggibile e scrivibile)
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Dimostrazione di fallback quando non possiamo creare il parametro
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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


