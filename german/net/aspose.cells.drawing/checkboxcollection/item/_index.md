---
title: "CheckBoxCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CheckBoxCollection-Eigenschaft. Gibt das CheckBox-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Ruft das [`CheckBox`](../../checkbox/) Element am angegebenen Index ab.

```csharp
public CheckBox this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein Kontrollkästchen zum Arbeitsblatt hinzu
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Greifen Sie auf das CheckBox über die Item-Eigenschaft (Indexer) zu
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Greifen Sie auf das CheckBox über den Index (Item-Eigenschaft) zu
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Geben Sie die CheckBox-Eigenschaften aus
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


