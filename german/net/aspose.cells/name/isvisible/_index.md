---
title: "Name.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt an, ob der Name sichtbar ist"
type: docs
url: /de/net/aspose.cells/name/isvisible/
---
## Name.IsVisible property

Gibt an, ob der Name sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen sichtbaren benannten Bereich
            int visibleIndex = workbook.Worksheets.Names.Add("VisibleRange");
            Name visibleName = workbook.Worksheets.Names[visibleIndex];
            visibleName.RefersTo = "=Sheet1!$A$1:$B$2";
            visibleName.IsVisible = true;
            
            // Erstellen Sie einen versteckten benannten Bereich
            int hiddenIndex = workbook.Worksheets.Names.Add("HiddenRange");
            Name hiddenName = workbook.Worksheets.Names[hiddenIndex];
            hiddenName.RefersTo = "=Sheet1!$C$1:$D$2";
            hiddenName.IsVisible = false;
            
            // Demonstrieren Sie die IsVisible-Eigenschaft
            Console.WriteLine("VisibleRange IsVisible: " + visibleName.IsVisible);
            Console.WriteLine("HiddenRange IsVisible: " + hiddenName.IsVisible);
            
            // Speichere die Arbeitsmappe
            workbook.Save("NameVisibilityDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


