---
title: "VbaModuleCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-egenskapen. Hämtar VbaModule i listan efter index"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Hämtar [`VbaModule`](../../vbamodule/) i listan efter index.

```csharp
public VbaModule this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med VBA-projekt
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Hämta befintligt VBA-projekt (VbaProject är skrivskyddat)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en modul i VBA-projektet
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Kom åt modulen med Item-egenskapen
            VbaModule module = vbaProject.Modules[index];
            
            // Lägg till lite VBA-kod i modulen
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Spara arbetsboken
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Se även

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Hämtar [`VbaModule`](../../vbamodule/) i listan efter namn.

```csharp
public VbaModule this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på modulen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till VBA-modul i arbetsboken
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Kom åt modulen med Item-egenskapen efter namn
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // Ange VBA-kod
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Spara arbetsboken
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Verifiera genom att ladda tillbaka
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Se även

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


