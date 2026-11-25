---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Indica se il primo foglio di lavoro contiene variabili personalizzate"
type: docs
url: /it/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Indica se il primo foglio di lavoro contiene variabili personalizzate.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà WorkbookDesigner.VariablesWorksheetName. Questa proprietà sarà rimossa 3 mesi dopo, a partire da settembre 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Crea un foglio di lavoro di esempio
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per rendere l'esempio significativo
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visualizza il valore corrente della proprietà ContainsVariables
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Imposta la proprietà ContainsVariables su true
                designer.ContainsVariables = true;

                // Visualizza il valore aggiornato
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Salva il risultato
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


