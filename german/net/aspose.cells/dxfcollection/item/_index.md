---
title: "DxfCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DxfCollection-Eigenschaft. Gibt das Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Liest das Element am angegebenen Index.

```csharp
public Style this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der angegebene Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greife auf die DxfCollection aus der Arbeitsmappe zu
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Erstelle einen neuen Stil (kann nicht direkt zu DxfCollection hinzugefügt werden, da es keine Add-Methode hat)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Stil wird automatisch zur Sammlung hinzugefügt, wenn er erstellt wird

            // Hole das erste Element aus DxfCollection mithilfe der Item-Eigenschaft
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Ändere den Stil über die Item-Eigenschaft (da sie eine Referenz zurückgibt)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Die Änderung überprüfen
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Wende den Stil auf eine Zelle an, um die Wirkung zu sehen
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Ergebnis speichern
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


