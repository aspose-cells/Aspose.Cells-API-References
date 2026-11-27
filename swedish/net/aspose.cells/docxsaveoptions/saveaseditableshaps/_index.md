---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DocxSaveOptions‑egenskap. Spara alla ritobjekt som redigerbara former i Word‑fil. Så kan du redigera dem i Word"
type: docs
url: /sv/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Spara alla ritobjekt som redigerbara former i Word‑fil. Så kan du redigera dem i Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Anmärkningar

OBS: Den här medlemmen är nu föråldrad. Använd istället [`SaveAsEditableShapes`](../saveaseditableshapes/) egenskap. Denna egenskap kommer att tas bort 6 månader senare, sedan maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Skapa ett arbetsbok‑objekt och öppna mall‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");

            // Initiera DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Ställ in egenskapen SaveAsEditableShaps till true
            saveOptions.SaveAsEditableShaps = true;

            // Spara arbetsboken som DOCX med de angivna alternativen
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Se även

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


