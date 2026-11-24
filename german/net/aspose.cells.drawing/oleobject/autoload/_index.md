---
title: "OleObject.AutoLoad"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt an, ob die Host-Anwendung für das eingebettete Objekt automatisch aufgerufen werden soll, um die Objektdaten zu laden, wenn die übergeordnete Arbeitsmappe geöffnet wird."
type: docs
url: /de/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Gibt an, ob die Host-Anwendung für das eingebettete Objekt automatisch aufgerufen werden soll, um die Objektdaten zu laden, wenn die übergeordnete Arbeitsmappe geöffnet wird.

```csharp
public bool AutoLoad { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ein OleObject zum Arbeitsblatt hinzufügen
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // OleObject-Eigenschaften festlegen
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // AutoLoad-Eigenschaft demonstrieren
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


