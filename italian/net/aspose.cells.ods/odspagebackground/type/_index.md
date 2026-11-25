---
title: "OdsPageBackground.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta il tipo di sfondo della pagina"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

Ottiene e imposta il tipo di sfondo della pagina.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alla configurazione della pagina del primo foglio di lavoro
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // Ottieni lo sfondo della pagina ODS
            OdsPageBackground background = ps.ODSPageBackground;
            
            // Imposta il tipo di sfondo su grafico e configurarlo
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // Salva la cartella di lavoro
            workbook.Save("output.ods");
            
            // Ricarica il file salvato per verificare le impostazioni
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // Emetti i risultati della verifica
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### Vedi anche

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


