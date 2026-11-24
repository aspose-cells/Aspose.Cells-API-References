---
title: "ExternalLinkCollection.Clear"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExternalLinkCollection-Methode. Entfernt alle externen Links"
type: docs
url: /de/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Entfernt alle externen Links.

```csharp
public void Clear()
```

### Hinweise

Beim Entfernen externer Links werden alle Formeln, die darauf verweisen, ebenfalls entfernt, weil die Verweise ungültig werden.

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Entfernt alle externen Links.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Ob alle Verweise externer Links in Formeln auf die Verweise der aktuellen Arbeitsmappe selbst aktualisiert werden sollen. |

### Hinweise

Wenn Verweise aktualisiert werden müssen, werden die Verweise externer Links in Formeln, sofern möglich, auf die aktuelle Arbeitsmappe geändert. Zum Beispiel lautet die ursprüngliche Formel einer Zelle "='externalsource.xlam'!customfunction()", nach dem Entfernen externer Links wird die Formel zu "=customfunction()". Wenn die ursprüngliche Formel "='[externalsource.xlam]Sheet1'!$A$1" lautet, hängt die Umwandlung davon ab, ob im aktuellen Arbeitsblatt ein Blatt mit dem Namen "Sheet1" existiert: Ist dies der Fall, wird die Formel zu "=Sheet1!$A$1"; ist es nicht der Fall, wird die Formel zu "=#REF!$A$1". Wenn Verweise nicht aktualisiert werden müssen, werden alle Formeln mit Verweisen zu externen Links ebenfalls entfernt, weil diese Verweise ungültig werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Füge einige externe Links hinzu
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Clear mit updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Füge Links erneut hinzu
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Clear mit updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Siehe auch

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


