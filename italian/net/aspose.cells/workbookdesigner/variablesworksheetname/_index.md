---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookDesigner. Ottiene e imposta il nome del foglio di lavoro che contiene il marcatore intelligente delle variabili"
type: docs
url: /it/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Ottiene e imposta il nome del foglio di lavoro che contiene variabili smart marker.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyVariablesWorksheetNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un nuovo workbook
                Workbook workbook = new Workbook();

                // Aggiungi un foglio di lavoro chiamato "Variables" per dimostrare la proprietà
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Crea un'istanza di WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visualizza il valore corrente di VariablesWorksheetName
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Imposta un nuovo valore per VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Aggiungi un altro foglio di lavoro con marcatori intelligenti
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Elabora i marcatori intelligenti
                designer.Process();

                // Salva la cartella di lavoro
                workbook.Save("VariablesWorksheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with VariablesWorksheetName set.");
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


