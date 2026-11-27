---
title: "WorkbookDesigner.ContainsVariables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookDesigner‑egenskap. Anger om det första kalkylbladet innehåller anpassade variabler"
type: docs
url: /sv/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

Anger om det första kalkylbladet innehåller anpassade variabler.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd i stället WorkbookDesigner.VariablesWorksheetName‑egenskapen. Denna egenskap kommer att tas bort 3 månader senare, från och med september 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en WorkbookDesigner‑instans
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // Visa det aktuella värdet för ContainsVariables‑egenskapen
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // Ställ in ContainsVariables‑egenskapen till true
                designer.ContainsVariables = true;

                // Visa det uppdaterade värdet
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // Spara resultatet
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

### Se även

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


