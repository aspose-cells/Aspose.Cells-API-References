---
title: "ExternalLinkCollection.Clear"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLinkCollection‑metod. Tar bort alla externa länkar"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

Tar bort alla externa länkar.

```csharp
public void Clear()
```

### Anmärkningar

När externa länkar tas bort kommer alla formler som refererar till dem också att tas bort eftersom referenserna blir ogiltiga.

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

Tar bort alla externa länkar.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| updateReferencesAsLocal | Boolean | Om alla referenser till externa länkar i formler ska uppdateras till referenser till den aktuella arbetsboken själv. |

### Anmärkningar

Om referenser ska uppdateras kommer de referenser till externa länkar i formler att ändras till den aktuella arbetsboken när det är möjligt. Till exempel är en cells ursprungliga formel "='externalsource.xlam'!customfunction()", efter att externa länkar tagits bort blir formeln "=customfunction()"; När den ursprungliga formeln är "='[externalsource.xlam]Sheet1'!$A$1", beroende på om det finns ett blad med namnet "Sheet1" i den aktuella arbetsboken: om sant blir formeln "=Sheet1!$A$1"; om falskt blir formeln "=#REF!$A$1". Om referenser inte ska uppdateras tas alla formler med referenser till externa länkar också bort eftersom dessa referenser blir ogiltiga.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några externa länkar
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // Clear med updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // Lägg till länkar igen
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // Clear med updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


