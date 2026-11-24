---
title: "WorkbookDesigner.VariablesWorksheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner-Eigenschaft. Liest und schreibt den Namen des Arbeitsblatts, das die Variablen‑Smart‑Marker enthält"
type: docs
url: /de/net/aspose.cells/workbookdesigner/variablesworksheetname/
---
## WorkbookDesigner.VariablesWorksheetName property

Liest und setzt den Namen des Arbeitsblatts, das Variablen‑Smart‑Marker enthält.

```csharp
public string VariablesWorksheetName { get; set; }
```

### Beispiele

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
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();

                // Ein Arbeitsblatt mit dem Namen "Variables" hinzufügen, um die Eigenschaft zu demonstrieren
                Worksheet variablesSheet = workbook.Worksheets.Add("Variables");
                variablesSheet.Cells["A1"].PutValue("Variable1");
                variablesSheet.Cells["B1"].PutValue("Value1");

                // Erstellen Sie eine WorkbookDesigner‑Instanz
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Den aktuellen Wert von VariablesWorksheetName anzeigen
                Console.WriteLine("Initial VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Setzen Sie einen neuen Wert für VariablesWorksheetName
                designer.VariablesWorksheetName = "Variables";
                Console.WriteLine("Updated VariablesWorksheetName: " + designer.VariablesWorksheetName);

                // Fügen Sie ein weiteres Arbeitsblatt mit Smart-Markern hinzu
                Worksheet templateSheet = workbook.Worksheets.Add("Template");
                templateSheet.Cells["A1"].PutValue("&=$Variable1");

                // Verarbeiten Sie die Smart-Marker
                designer.Process();

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


