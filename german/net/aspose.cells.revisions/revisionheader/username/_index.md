---
title: "RevisionHeader.UserName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionHeader-Eigenschaft. Gibt den Namen des Benutzers zurück, der die Revision vornimmt, und legt ihn fest"
type: docs
url: /de/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Liest und setzt den Namen des Benutzers, der die Revision vornimmt.

```csharp
public string UserName { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            try
            {
                // Erstellen Sie eine RevisionHeader-Instanz
                RevisionHeader revisionHeader = new RevisionHeader();

                // Setzen Sie die UserName-Eigenschaft
                revisionHeader.UserName = "JohnDoe";

                // Zeigen Sie den aktuellen Wert der UserName-Eigenschaft an
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Ändern Sie die UserName-Eigenschaft
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Speichern Sie die Arbeitsmappe, um zu demonstrieren, dass die Eigenschaft verwendet wird
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


