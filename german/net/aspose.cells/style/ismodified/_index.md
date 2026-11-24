---
title: "Style.IsModified"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Prüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils beim Anwenden von ConditionalFormattings auf eine Zelle verwendet werden sollen."
type: docs
url: /de/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Überprüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils verwendet werden sollten, wenn ConditionalFormattings auf eine Zelle angewendet werden.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Stil-Änderungsflags |

### Rückgabewert

wahr, wenn die angegebenen Eigenschaften geändert wurden

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hole den Stil der Zelle A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Das Muster (Hintergrund) des Stils ändern
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Prüfen, ob das Muster geändert wurde
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Siehe auch

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


