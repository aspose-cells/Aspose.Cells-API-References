---
title: "ListObject.ApplyStyleToRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Methode. Wendet den Tabellenstil auf den Bereich an"
type: docs
url: /de/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Wendet die Tabellenformatvorlage auf den Bereich an.

```csharp
public void ApplyStyleToRange()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um ein List-Objekt zu erstellen.
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Stil auf den Bereich des ListObject anwenden
            listObject.ApplyStyleToRange();

            // Überprüfen, ob der Stil angewendet wurde, indem die Vordergrundfarbe einer Zelle geprüft wird
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // ListObject in Bereich konvertieren und prüfen
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


