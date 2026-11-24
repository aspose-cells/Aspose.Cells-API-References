---
title: "VbaModuleCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Eigenschaft. Gibt VbaModule in der Liste nach dem Index zurück"
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Gibt [`VbaModule`](../../vbamodule/) in der Liste nach dem Index zurück.

```csharp
public VbaModule this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe mit VBA-Projekt
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Vorhandenes VBA-Projekt abrufen (VbaProject ist schreibgeschützt)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Fügen Sie ein Modul zum VBA-Projekt hinzu
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Greifen Sie über die Item-Eigenschaft auf das Modul zu
            VbaModule module = vbaProject.Modules[index];
            
            // Füge dem Modul etwas VBA-Code hinzu
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Speichere die Arbeitsmappe
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Gibt [`VbaModule`](../../vbamodule/) in der Liste nach dem Namen zurück.

```csharp
public VbaModule this[string name] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Name | Der Name des Moduls. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // VBA-Modul zum Arbeitsbuch hinzufügen
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Zugriff auf das Modul über die Item-Eigenschaft nach Name
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // VBA-Code festlegen
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Durch erneutes Laden verifizieren
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Siehe auch

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


