---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormulaItemCollection. Obtiene PowerQueryFormulaItem por el índice en la lista"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Obtiene [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) por el índice en la lista.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
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
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con una plantilla que contiene Power Query
            Workbook workbook = new Workbook();
            
            // Obtener la primera fórmula de Power Query (asumiendo que exista)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Modificar los elementos de la fórmula usando la propiedad Item
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Verificar el cambio
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Obtiene [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) por el nombre del elemento.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del elemento. |

### Ejemplos

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
                // Cargar un libro de trabajo que contiene fórmulas de Power Query.
                // Reemplazar la ruta con un archivo real que contenga Power Query si está disponible.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Acceder a la colección de fórmulas de Power Query.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Obtener la primera fórmula de Power Query.
                PowerQueryFormula formula = pqFormulas[0];

                // Acceder a su colección de elementos.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Recuperar el primer elemento para obtener un nombre de elemento válido.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Usar el indexador Item(string) (solo lectura) para obtener el mismo elemento por nombre.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Mostrar las propiedades del elemento recuperado.
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

### Ver también

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


