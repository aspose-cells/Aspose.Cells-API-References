---
title: "Classe DataMashup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.QueryTables.DataMashup. Rappresenta i dati mashup"
type: docs
url: /it/net/aspose.cells.querytables/datamashup/
---
## DataMashup class

Rappresenta i dati mashup.

```csharp
public class DataMashup
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PowerQueryFormulaParameters](../../aspose.cells.querytables/datamashup/powerqueryformulaparameters/) { get; } | (**Obsoleto.**) Ottiene i parametri della formula Power Query. |
| [PowerQueryFormulas](../../aspose.cells.querytables/datamashup/powerqueryformulas/) { get; } | Ottiene tutte le formule Power Query. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class DataMashupDemo
    {
        public static void DataMashupExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla proprietà DataMashup della cartella di lavoro
            DataMashup dataMashup = workbook.DataMashup;

            if (dataMashup != null )
            {
                // Accedi alla proprietà PowerQueryFormulas
                var powerQueryFormulas = dataMashup.PowerQueryFormulas;

                // Accedi alla proprietà PowerQueryFormulaParameters
                var powerQueryFormulaParameters = dataMashup.PowerQueryFormulaParameters;

                // Esempio di utilizzo: iterare attraverso PowerQueryFormulas
                foreach (var formula in powerQueryFormulas)
                {
                    Console.WriteLine(formula.Name);
                }

                // Esempio di utilizzo: iterare attraverso PowerQueryFormulaParameters
                foreach (var parameter in powerQueryFormulaParameters)
                {
                    Console.WriteLine(parameter.Name);
                }
            }
            

            // Salva la cartella di lavoro
            workbook.Save("DataMashupExample.xlsx");
            workbook.Save("DataMashupExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


