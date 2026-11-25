---
title: "OdsPageBackground.GraphicData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta i dati della grafica"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

Ottiene e imposta i dati grafici.

```csharp
public byte[] GraphicData { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e alla sua configurazione di pagina
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Imposta le proprietà di sfondo della pagina ODS
            OdsPageBackground background = pageSetup.ODSPageBackground;
            background.Type = OdsPageBackgroundType.Graphic;
            
            // Carica i dati dell'immagine e impostali come sfondo
            string imagePath = "sample.png"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                background.GraphicData = File.ReadAllBytes(imagePath);
                background.GraphicType = OdsPageBackgroundGraphicType.Area;
                
                // Salva la cartella di lavoro
                workbook.Save("output.ods");
                
                Console.WriteLine("ODS file with graphic background created successfully.");
            }
            else
            {
                Console.WriteLine("Image file not found: " + imagePath);
            }
        }
    }
}
```

### Vedi anche

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


