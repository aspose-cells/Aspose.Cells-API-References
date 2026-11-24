---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookDesigner‑Eigenschaft. Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält"
type: docs
url: /de/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft WorkbookDesigner.VariablesWorksheetName. Diese Eigenschaft wird 3 Monate nach September 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Erstelle ein Beispiel-Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Erstellen Sie eine WorkbookDesigner‑Instanz
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Zeigen Sie den aktuellen Wert der ContainsVariables‑Eigenschaft an
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Setzen Sie die ContainsVariables‑Eigenschaft auf true
                designer.ContainsVariables = true;

                // Zeigen Sie den aktualisierten Wert an
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Ergebnis speichern
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

### Siehe auch

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


