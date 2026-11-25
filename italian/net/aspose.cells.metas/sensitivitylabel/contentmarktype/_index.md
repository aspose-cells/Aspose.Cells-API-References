---
title: "SensitivityLabel.ContentMarkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SensitivityLabel. Ottiene e imposta i tipi di marcatura del contenuto che devono essere applicati a un file"
type: docs
url: /it/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Ottiene e imposta i tipi di marcatura del contenuto che dovrebbero essere applicati a un file.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Creare un'istanza di SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Imposta le proprietà di base
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Dimostrare la proprietà ContentMarkType (lettura-scrittura)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Impostare diversi tipi di marcatura del contenuto
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Mostrare l'uso di flag combinati
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Salva la cartella di lavoro
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

### Vedi anche

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


