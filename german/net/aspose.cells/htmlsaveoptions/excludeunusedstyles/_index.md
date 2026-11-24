---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob nicht verwendete Stile ausgeschlossen werden. Für die erzeugten HTML-Dateien kann das Ausschließen nicht verwendeter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss, z. B. im Szenario, dass die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll, setzen Sie diese Eigenschaft bitte auf false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Gibt an, ob ungenutzte Stile ausgeschlossen werden. Bei den erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn das Arbeitsblatt später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft bitte auf false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Beispieldaten mit unterschiedlichen Stilen hinzufügen
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // HTML-Speicheroptionen konfigurieren, um nicht verwendete Stile auszuschließen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Speichere die Arbeitsmappe mit HTML-Optionen
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


