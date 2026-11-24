---
title: "WorksheetCollection.CreateUnionRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorksheetCollection-Methode. Erstellt ein Range-Objekt aus einer Adresse des Bereichs"
type: docs
url: /de/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

Erstellt ein [`Range`](../../range/) Objekt aus einer Adresse des Bereichs.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| address | String | Die Adresse des Bereichs. |
| sheetIndex | Int32 | Der Blattindex. |

### Rückgabewert

Ein [`Range`](../../range/) Objekt

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Unionbereich aus Adresszeichenfolgen
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // Setze den Wert für den gesamten Vereinigungsbereich
            unionRange.Value = "Test";
            
            // Wende Styling auf den Unionbereich an
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // Speichere die Arbeitsmappe
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


