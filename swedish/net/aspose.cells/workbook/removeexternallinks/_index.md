---
title: "Workbook.RemoveExternalLinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Tar bort alla externa länkar i arbetsboken"
type: docs
url: /sv/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

Tar bort alla externa länkar i arbetsboken.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ExternalLinkCollection.Clear()‑metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2021. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Anropa RemoveExternalLinks‑metoden
                workbook.RemoveExternalLinks();

                // Visa resultat eller effekter av metodanropet
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // Spara arbetsboken om ändringar har gjorts
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


