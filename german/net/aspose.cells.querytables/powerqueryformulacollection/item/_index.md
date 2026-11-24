---
title: "PowerQueryFormulaCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaCollection‑Eigenschaft. Ruft PowerQueryFormula anhand des Index in der Liste ab"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Ruft [`PowerQueryFormula`](../../powerqueryformula/) anhand des Index in der Liste ab.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Power‑Query‑Formeln abrufen
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Erstellen und fügen Sie eine neue Formel hinzu (falls nötig)
            // Hinweis: Die tatsächliche Implementierung könnte einen anderen Ansatz zum Hinzufügen von Formeln erfordern
            // Zu Demonstrationszwecken arbeiten wir mit vorhandenen Formeln, falls vorhanden.
            if (formulas.Count == 0)
            {
                // Dies dient nur zur Demonstration – die tatsächliche API könnte einen anderen Ansatz erfordern.
                // um neue Formeln zu erstellen
                return;
            }

            // Zugriff auf die erste Formel über die Eigenschaft Item
            var formula = formulas[0];
            
            // Formelelemente abrufen
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Dies dient nur zur Demonstration – die tatsächliche API könnte einen anderen Ansatz erfordern.
                // um neue Formelelemente zu erstellen
                return;
            }

            // Zugriff auf das erste Element über die Eigenschaft Item
            var formulaItem = formulaItems[0];
            
            // Wert setzen und abrufen über die Eigenschaft Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Liefert [`PowerQueryFormula`](../../powerqueryformula/) anhand des Namens der Power‑Query‑Formel.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name des Elements. |

### Beispiele

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
            // Erstelle eine Arbeitsmappe, indem du eine vorhandene Datei lädst, die Power‑Query‑Formeln enthält
            Workbook workbook = new Workbook("example.xlsx");
            
            // Power‑Query‑Formelsammlung abrufen
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Demonstriere die Verwendung der Item-Eigenschaft
            try
            {
                // Versuche, auf eine vorhandene Formel zuzugreifen (falls vorhanden)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Dies löst eine Ausnahme für eine nicht vorhandene Formel aus
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

### Siehe auch

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


