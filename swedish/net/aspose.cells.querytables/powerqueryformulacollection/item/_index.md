---
title: "PowerQueryFormulaCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaCollection-egenskap. Hämtar PowerQueryFormula efter index i listan"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Hämtar [`PowerQueryFormula`](../../powerqueryformula/) efter index i listan.

```csharp
public PowerQueryFormula this[int index] { get; }
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
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Hämta Power Query-formler
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Skapa och lägg till en ny formel (om det behövs)
            // Obs: Den faktiska implementeringen kan kräva ett annat tillvägagångssätt för att lägga till formler
            // För demonstrationsändamål kommer vi att arbeta med befintliga formler om några finns
            if (formulas.Count == 0)
            {
                // Detta är bara för demonstration - den faktiska API:n kan kräva ett annat tillvägagångssätt
                // för att skapa nya formler
                return;
            }

            // Åtkomst till den första formeln med Item‑egenskapen
            var formula = formulas[0];
            
            // Hämta formelobjekt
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Detta är bara för demonstration - den faktiska API:n kan kräva ett annat tillvägagångssätt
                // för att skapa nya formelobjekt
                return;
            }

            // Åtkomst till det första objektet med Item‑egenskapen
            var formulaItem = formulaItems[0];
            
            // Ställ in och hämta värde med Item‑egenskapen
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Demonstrera användning av Item-egenskapen
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Spara arbetsboken
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Se även

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Hämtar [`PowerQueryFormula`](../../powerqueryformula/) efter namnet på Power Query-formeln.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på objektet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en arbetsbok genom att läsa in en befintlig fil som innehåller Power Query-formler
            Workbook workbook = new Workbook("example.xlsx");
            
            // Hämta samling av Power Query-formler
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Demonstrera användning av Item-egenskapen
            try
            {
                // Försök att komma åt en befintlig formel (om någon finns)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Detta kommer att kasta ett undantag för en icke‑existerande formel
                PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


