---
title: "PowerQueryFormula.GroupName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormula property. Hämtar namnet på gruppen som innehåller denna Power Query-formel"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

Hämtar namnet på gruppen som innehåller denna Power Query-formel.

```csharp
public string GroupName { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en Power Query-formel (simulerad eftersom vi inte kan skapa faktiska PowerQueryFormulas direkt)
            // Normalt skulle du läsa in från en befintlig fil med Power Query-formler
            string sourcePath = "example.xlsx";
            
            try
            {
                workbook = new Workbook(sourcePath);
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                
                if (queries.Count > 0)
                {
                    Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
                    
                    // Demonstrera åtkomst till egenskapen GroupName
                    string groupName = queries[0].GroupName;
                    Console.WriteLine($"Group Name: {groupName}");
                    
                    // Spara och ladda om för att demonstrera beständighet
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

### Se även

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


