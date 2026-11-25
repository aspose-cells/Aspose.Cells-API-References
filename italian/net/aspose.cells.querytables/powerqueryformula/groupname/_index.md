---
title: "PowerQueryFormula.GroupName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormula. Ottiene il nome del gruppo che contiene questa formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

Ottiene il nome del gruppo che contiene questa formula Power Query.

```csharp
public string GroupName { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una formula Power Query (simulata poiché non possiamo creare PowerQueryFormulas reali direttamente)
            // Normalmente caricheresti da un file esistente con formule Power Query
            string sourcePath = "example.xlsx";
            
            try
            {
                workbook = new Workbook(sourcePath);
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                
                if (queries.Count > 0)
                {
                    Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
                    
                    // Dimostra l'accesso alla proprietà GroupName
                    string groupName = queries[0].GroupName;
                    Console.WriteLine($"Group Name: {groupName}");
                    
                    // Salva e ricarica per dimostrare la persistenza
                    string destPath = "output.xlsx";
                    workbook.Save(destPath);
                    
                    Workbook workbook2 = new Workbook(destPath);
                    PowerQueryFormulaCollection queries2 = workbook2.DataMashup.PowerQueryFormulas;
                    if (queries2.Count > 0)
                    {
                        Console.WriteLine("After reload - Group Name: " + queries2[0].GroupName);
                    }
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the file.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


