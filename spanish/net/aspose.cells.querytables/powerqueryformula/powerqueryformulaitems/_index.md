---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PowerQueryFormula. Obtiene todos los elementos de la fórmula Power Query"
type: docs
url: /es/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Obtiene todos los elementos de la fórmula de Power Query.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Ejemplos

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
            // Cargar el libro de trabajo de origen
            Workbook workbook = new Workbook("example.xlsx");

            // Acceder a la primera fórmula Power Query y su primer elemento
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Modificar el valor del elemento (reemplazar la letra de la unidad)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Guarda el libro de trabajo
            workbook.Save("modified_example.xlsx");

            // Verificar el cambio
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### Ver también

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


