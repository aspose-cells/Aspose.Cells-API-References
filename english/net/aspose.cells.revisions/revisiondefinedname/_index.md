---
title: Class RevisionDefinedName
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Revisions.RevisionDefinedName class. Represents a revision record of a defined name change
type: docs
url: /net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Represents a revision record of a defined name change.

```csharp
public class RevisionDefinedName : Revision
```

## Properties

| Name | Description |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Gets the number of this revision.(Inherited from [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Gets the formula. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Gets the old formula. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Gets the text of the defined name. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Represents the type of revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Gets the worksheet.(Inherited from [`Revision`](../revision/).) |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add a defined name to the workbook
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modify the defined name to create a revision
                definedName.RefersTo = "=Sheet1!$B$1";

                // Save the workbook to generate revision logs
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Reopen the workbook to access revision information
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iterate through revision logs to find RevisionDefinedName entries
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Display the properties of the RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


