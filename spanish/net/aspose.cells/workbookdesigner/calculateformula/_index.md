---
title: "WorkbookDesigner.CalculateFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Indica si las fórmulas deben calcularse"
type: docs
url: /es/net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Indica si las fórmulas deben calcularse.

```csharp
public bool CalculateFormula { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con una fórmula
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y fórmula
            worksheet.Cells["A1"].PutValue("Opportunity Name");
            worksheet.Cells["B1"].PutValue("Opportunity Amount");
            worksheet.Cells["A2"].PutValue("=Master.Opportunity_Name");
            worksheet.Cells["B2"].PutValue("=Master.Opportunity_Amount");
            worksheet.Cells["C2"].Formula = "=CONCATENATE(A2,B2)";

            // Crear origen de datos
            DataTable dt = new DataTable("Master");
            dt.Columns.Add("Opportunity_Name");
            dt.Columns.Add("Opportunity_Amount");
            DataRow dr = dt.NewRow();
            dr["Opportunity_Name"] = "Test Deal";
            dr["Opportunity_Amount"] = "$2500.00";
            dt.Rows.Add(dr);

            // Procesar el diseñador con CalculateFormula habilitado
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            designer.SetDataSource(dt);
            designer.CalculateFormula = true; // This will calculate formulas after data binding
            designer.Process();

            // Mostrar el resultado
            Console.WriteLine("Formula result: " + worksheet.Cells["C2"].StringValue);
        }
    }
}
```

### Ver también

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


