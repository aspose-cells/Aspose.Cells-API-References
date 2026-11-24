---
title: "Aufzählung VbaModuleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Vba.VbaModuleType-Enum. Stellt den Typ eines VBA-Moduls dar"
type: docs
url: /de/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Stellt den Typ des VBA‑Moduls dar.

```csharp
public enum VbaModuleType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Procedural | `0` | Stellt ein prozedurales Modul dar. |
| Document | `1` | Stellt ein Dokumentmodul dar. |
| Class | `2` | Stellt ein Klassenmodul dar. |
| Designer | `3` | Stellt ein Designermodul dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // VBA-Projekt initialisieren
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ein neues Klassenmodul hinzufügen
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Das VBA-Modul abrufen
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Codes für das Modul festlegen
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Speichere die Excel-Datei
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


