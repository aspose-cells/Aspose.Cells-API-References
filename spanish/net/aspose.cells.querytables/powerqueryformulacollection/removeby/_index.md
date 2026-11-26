---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PowerQueryFormulaCollection. Eliminar fórmula de Power Query por nombre"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Elimina la fórmula de Power Query por nombre.

```csharp
public void RemoveBy(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la fórmula de Power Query. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Acceder a PowerQueryFormulaCollection (suponiendo que exista en el libro de trabajo)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Agregar una fórmula de ejemplo para eliminar (normalmente provendría de datos existentes)
                string formulaName = "SampleFormula";
                
                // Llamar a RemoveBy con el nombre de la fórmula
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Guarda el libro de trabajo
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


