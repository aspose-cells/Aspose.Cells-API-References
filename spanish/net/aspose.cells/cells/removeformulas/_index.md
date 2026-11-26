---
title: "Cells.RemoveFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina todas las fórmulas y las reemplaza con el valor de la fórmula"
type: docs
url: /es/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Elimina todas las fórmulas y las reemplaza con el valor de la fórmula.

```csharp
public void RemoveFormulas()
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // Crear un conjunto de datos de ejemplo
            DataSet ds = new DataSet();

            // Crear y rellenar la tabla Master
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // Crear y rellenar la tabla OppLineItems
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Crear un nuevo libro de trabajo
            Workbook wkb = new Workbook();
            
            // Usar WorkbookDesigner para enlazar datos
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Agregar una fórmula para demostrar la eliminación
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Calcular fórmulas primero
            wkb.CalculateFormula();

            // Eliminar todas las fórmulas de la hoja de cálculo
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Guarda el libro de trabajo
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


