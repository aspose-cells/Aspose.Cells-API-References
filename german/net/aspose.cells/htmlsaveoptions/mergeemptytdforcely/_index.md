---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob leere TD-Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Größe der HTML-Datei wird nach dem Setzen des Wertes auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML-Datei in Excel importieren oder beim Speichern der Datei nach HTML perfekte Rasterlinien exportieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Gibt an, ob leere TD-Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Größe der HTML-Datei wird nach dem Setzen des Wertes auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML-Datei in Excel importieren oder beim Speichern der Datei nach HTML perfekte Rasterlinien exportieren möchten, behalten Sie bitte den Standardwert bei.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Ein Beispielarbeitsbuch mit leeren Zellen erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige leere Zellen im Arbeitsblatt erstellen
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 ist absichtlich leer gelassen
            
            // Speichern mit aktiviertem MergeEmptyTdForcely
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Speichern ohne MergeEmptyTdForcely zum Vergleich
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


