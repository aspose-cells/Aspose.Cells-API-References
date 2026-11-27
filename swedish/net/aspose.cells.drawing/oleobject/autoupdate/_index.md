---
title: "OleObject.AutoUpdate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OleObject-egenskap. Anger om länken till OleObject uppdateras automatiskt eller inte"
type: docs
url: /sv/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Anger om länken till OleObject uppdateras automatiskt eller inte.

```csharp
public bool AutoUpdate { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempel-filer för demonstration
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Skapa exempelbildfil om den inte finns
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Skapa exempel-Excel-fil om den inte finns
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Läs bilddata
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Lägg till OleObject i kalkylbladet
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Ange OleObject-egenskaper
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // Demonstrera AutoUpdate-egenskapen
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Spara arbetsboken
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


