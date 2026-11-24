---
title: "VbaProject.Protect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaProject-Methode. Schützt oder hebt den Schutz dieses VBA-Projekts auf"
type: docs
url: /de/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Schützt oder hebt den Schutz dieses VBA-Projekts auf.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| islockedForViewing | Boolean | Gibt an, ob das Projekt für die Ansicht gesperrt ist. |
| Passwort | String | Wenn der Wert null ist, wird der Schutz dieses VBA-Projekts aufgehoben, andernfalls wird das Projekt geschützt. |

### Hinweise

Wenn islockedForViewing true ist, darf das Passwort nicht null sein.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


