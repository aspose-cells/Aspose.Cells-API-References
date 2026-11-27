---
title: "SensitivityLabel.ContentMarkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SensitivityLabel‑egenskapen. Hämtar och anger typerna av innehållsmarkering som ska tillämpas på en fil"
type: docs
url: /sv/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Hämtar och anger typerna av innehållsmärkning som ska tillämpas på en fil.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Skapa en instans av sensitivity label
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Ställ in grundläggande egenskaper
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Demonstrera ContentMarkType‑egenskapen (läslig/skrivbar)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Ange olika innehållsmarkeringstyper
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Visa användning av kombinerade flaggor
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Spara arbetsboken
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

### Se även

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


