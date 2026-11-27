---
title: "VbaProject.Protect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaProject metod. Skyddar eller avskyddar detta VBA-projekt"
type: docs
url: /sv/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Skyddar eller avskyddar detta VBA-projekt.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| islockedForViewing | Boolean | Indikerar om projektet är låst för visning. |
| lösenord | String | Om värdet är null avskyddar den här VBA-projektet, annars skyddar den här VBA-projektet. |

### Anmärkningar

Om islockedForViewing är true får lösenordet inte vara null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med VBA-projekt
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Spara arbetsboken
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


