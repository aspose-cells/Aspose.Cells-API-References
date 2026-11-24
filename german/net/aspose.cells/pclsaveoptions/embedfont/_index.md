---
title: "PclSaveOptions.EmbedFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PclSaveOptions-Eigenschaft. Gibt an, ob die Schriftart in die Ausgabedatei Pcl eingebettet werden soll."
type: docs
url: /de/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Gibt an, ob die Schriftart in die Ausgabedatei Pcl eingebettet werden soll.

```csharp
public bool EmbedFont { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und fügen Sie einige Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Erstelle PCL-Speicheroptionen
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Lesen und zeigen Sie den aktuellen Wert der EmbedFont-Eigenschaft an.
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Optional) Wenn die Eigenschaft schreibbar ist, könnten Sie sie setzen, aber wir lesen sie hier nur.
                // pclOptions.EmbedFont = true;

                // Speichern Sie die Arbeitsmappe als PCL-Datei unter Verwendung der Optionen.
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


