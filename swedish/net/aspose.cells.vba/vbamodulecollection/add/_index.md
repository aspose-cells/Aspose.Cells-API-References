---
title: "VbaModuleCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-metod. Lägger till modul för ett arbetsblad"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Lägger till modul för ett kalkylblad.

```csharp
public int Add(Worksheet sheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | Arbetsblad | Arbetsbladet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en VBA-modul som är kopplad till arbetsbladet
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Lägg till lite VBA-kod i modulen
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Spara arbetsboken med VBA-projekt
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Lägger till modul.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | VbaModuleType | Typen av modul. |
| namn | String | Namnet på modulen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### Se även

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


