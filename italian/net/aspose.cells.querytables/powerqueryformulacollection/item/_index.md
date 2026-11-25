---
title: "PowerQueryFormulaCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaCollection. Ottiene PowerQueryFormula per indice nella lista"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Ottiene [`PowerQueryFormula`](../../powerqueryformula/) per indice nella lista.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Ottieni formule Power Query
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Crea e aggiungi una nuova formula (se necessario)
            // Nota: L'implementazione reale potrebbe richiedere un approccio diverso per aggiungere formule
            // Per scopi dimostrativi, lavoreremo con le formule esistenti, se presenti
            if (formulas.Count == 0)
            {
                // Questo è solo a scopo dimostrativo - l'API reale potrebbe richiedere un approccio diverso
                // per creare nuove formule
                return;
            }

            // Accedi alla prima formula usando la proprietà Item
            var formula = formulas[0];
            
            // Ottieni gli elementi della formula
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Questo è solo a scopo dimostrativo - l'API reale potrebbe richiedere un approccio diverso
                // per creare nuovi elementi della formula
                return;
            }

            // Accedi al primo elemento usando la proprietà Item
            var formulaItem = formulaItems[0];
            
            // Imposta e ottieni il valore usando la proprietà Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Dimostra l'uso della proprietà Item
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Salva la cartella di lavoro
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Ottiene [`PowerQueryFormula`](../../powerqueryformula/) per nome della formula Power Query.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome dell'elemento. |

### Esempi

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
            // Crea una cartella di lavoro caricando un file esistente che contiene formule Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // Ottieni la collezione di formule Power Query
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Dimostra l'uso della proprietà Item
            try
            {
                // Prova ad accedere a una formula esistente (se presente)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Questo genererà un'eccezione per una formula inesistente
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

### Vedi anche

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


