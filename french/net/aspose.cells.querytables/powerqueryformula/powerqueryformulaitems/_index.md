---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PowerQueryFormula propriété. Obtient tous les éléments de la formule Power Query"
type: docs
url: /fr/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Obtient tous les éléments de la formule Power Query.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // Charger le classeur source
            Workbook workbook = new Workbook("example.xlsx");

            // Accéder à la première formule Power Query et à son premier élément
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Modifier la valeur de l'élément (remplacer la lettre du lecteur)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Enregistrez le classeur
            workbook.Save("modified_example.xlsx");

            // Vérifier le changement
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Voir aussi

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


