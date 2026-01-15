---
title: RevisionDefinedName.Type
second_title: Aspose.Cells for .NET API Reference
description: RevisionDefinedName property. Represents the type of revision
type: docs
url: /net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Represents the type of revision.

```csharp
public override RevisionType Type { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook and add a defined name
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Change the defined name to generate a revision record
                definedName.RefersTo = "=Sheet1!$B$1";

                // Save the workbook to embed revision information
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Re‑open the workbook to read the revision log
                Workbook revWb = new Workbook(filePath);

                // Iterate through revisions and display the Type of each RevisionDefinedName entry
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


