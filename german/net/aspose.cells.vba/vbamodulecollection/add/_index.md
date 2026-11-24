---
title: "VbaModuleCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Methode. Fügt ein Modul für ein Arbeitsblatt hinzu"
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Fügt ein Modul für ein Arbeitsblatt hinzu.

```csharp
public int Add(Worksheet sheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blatt | Arbeitsblatt | Das Arbeitsblatt |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ein VBA-Modul zum Arbeitsblatt hinzufügen
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Füge dem Modul etwas VBA-Code hinzu
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Speichere die Arbeitsmappe mit VBA-Projekt
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Fügt ein Modul hinzu.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | VbaModuleType | Der Typ des Moduls. |
| Name | String | Der Name des Moduls. |

### Beispiele

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

### Siehe auch

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


