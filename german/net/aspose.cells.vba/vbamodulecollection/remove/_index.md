---
title: "VbaModuleCollection.Remove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Methode. Entfernt das Modul für ein Arbeitsblatt"
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Entfernt ein Modul für ein Arbeitsblatt.

```csharp
public void Remove(Worksheet sheet)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Blatt | Arbeitsblatt | Das Arbeitsblatt |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein VBA-Modul zum Arbeitsblatt hinzu
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Abrufen der VBA-Modulsammlung
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Rufen Sie die Remove-Methode mit dem Arbeitsblatt-Parameter auf
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Überprüfen Sie, ob das Modul entfernt wurde
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
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

## Remove(string) {#remove_1}

Entfernt das Modul anhand des Namens.

```csharp
public void Remove(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Makro
            Workbook workbook = new Workbook();
            
            // Zugriff auf VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ein neues Modul hinzufügen
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Fügen Sie dem Modul Code hinzu
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Speichere die Arbeitsmappe
            workbook.Save("output_with_module.xlsm");
            
            // Entfernen Sie das Modul nach Namen
            vbaProject.Modules.Remove("TestModule");
            
            // Speichern Sie die Arbeitsmappe nach dem Entfernen
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Siehe auch

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


