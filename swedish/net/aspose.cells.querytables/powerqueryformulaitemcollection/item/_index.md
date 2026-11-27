---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaItemCollection-egenskap. Hämtar PowerQueryFormulaItem efter index i listan"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Hämtar [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) efter index i listan.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med en mall som innehåller Power Query
            Workbook workbook = new Workbook();
            
            // Hämta den första Power Query-formeln (förutsatt att en finns)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Modifiera formelobjekten med hjälp av Item-egenskapen
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Verifiera ändringen
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Spara arbetsboken
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Hämtar [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) efter namn på objektet.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på objektet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            try
            {
                // Läs in en arbetsbok som innehåller Power Query-formler.
                // Byt ut sökvägen mot en faktisk fil som innehåller Power Query om den finns tillgänglig.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Åtkomst till samlingen av Power Query-formler.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Hämta den första Power Query-formeln.
                PowerQueryFormula formula = pqFormulas[0];

                // Åtkomst till dess objektssamling.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Hämta det första objektet för att få ett giltigt objektnamn.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Använd indexeraren Item(string) (skrivskyddad) för att få samma objekt med namn.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Visa de hämtade objektets egenskaper.
                Console.WriteLine($"Item Name : {retrievedItem.Name}");
                Console.WriteLine($"Item Value: {retrievedItem.Value}");
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

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


