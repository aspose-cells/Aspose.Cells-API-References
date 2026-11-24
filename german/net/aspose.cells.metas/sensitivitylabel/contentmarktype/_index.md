---
title: "SensitivityLabel.ContentMarkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SensitivityLabel-Eigenschaft. Gibt die Arten der Inhaltskennzeichnung zurück und legt sie fest, die auf eine Datei angewendet werden sollen."
type: docs
url: /de/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Liest und setzt die Arten der Inhaltskennzeichnung, die auf eine Datei angewendet werden sollen.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Erstellen Sie eine Instanz von SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Grundlegende Eigenschaften festlegen
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Demonstrieren Sie die ContentMarkType-Eigenschaft (lesbar/schreibbar)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Setzen Sie verschiedene Inhaltskennzeichnungstypen
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Zeigen Sie die Verwendung kombinierter Flags
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Speichere die Arbeitsmappe
                workbook.Save("ContentMarkTypeDemo.xlsx");
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

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


