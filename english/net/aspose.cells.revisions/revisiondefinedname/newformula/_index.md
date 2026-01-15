---
title: RevisionDefinedName.NewFormula
second_title: Aspose.Cells for .NET API Reference
description: RevisionDefinedName property. Gets the formula
type: docs
url: /net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Gets the formula.

```csharp
public string NewFormula { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and add some data
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // Add a defined name that points to A1
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Change the defined name to generate a revision (now points to B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Save the workbook to embed revision information
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Reopen the workbook to read revision logs
                Workbook revWorkbook = new Workbook(fileName);

                // Iterate through revisions and display NewFormula
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
                        }
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


