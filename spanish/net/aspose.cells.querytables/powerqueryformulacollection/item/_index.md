---
title: "PowerQueryFormulaCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaCollection. Obtiene PowerQueryFormula por el índice en la lista"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Obtiene [`PowerQueryFormula`](../../powerqueryformula/) por el índice en la lista.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener fórmulas de Power Query
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Crear y agregar una nueva fórmula (si es necesario)
            // Nota: La implementación real puede requerir un enfoque diferente para agregar fórmulas
            // Para propósitos de demostración, trabajaremos con fórmulas existentes si las hay
            if (formulas.Count == 0)
            {
                // Esto es solo para demostración - la API real podría requerir un enfoque diferente
                // para crear nuevas fórmulas
                return;
            }

            // Acceder a la primera fórmula usando la propiedad Item
            var formula = formulas[0];
            
            // Obtener elementos de fórmula
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Esto es solo para demostración - la API real podría requerir un enfoque diferente
                // para crear nuevos ítems de fórmula
                return;
            }

            // Acceder al primer ítem usando la propiedad Item
            var formulaItem = formulaItems[0];
            
            // Establecer y obtener el valor usando la propiedad Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Demostrar el uso de la propiedad Item
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Guarda el libro de trabajo
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Obtiene [`PowerQueryFormula`](../../powerqueryformula/) por el nombre de la fórmula de Power Query.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del elemento. |

### Ejemplos

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
            // Crear un libro de trabajo cargando un archivo existente que contiene fórmulas de Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // Obtener colección de fórmulas de Power Query
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Demostrar el uso de la propiedad Item
            try
            {
                // Intenta acceder a una fórmula existente (si la hay)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Esto lanzará una excepción para una fórmula inexistente
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

### Ver también

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


