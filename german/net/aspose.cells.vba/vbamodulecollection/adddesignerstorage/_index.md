---
title: "VbaModuleCollection.AddDesignerStorage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VbaModuleCollection-Methode."
type: docs
url: /de/net/aspose.cells.vba/vbamodulecollection/adddesignerstorage/
---
## VbaModuleCollection.AddDesignerStorage method

```csharp
public void AddDesignerStorage(string name, byte[] data)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String |  |
| Daten | Byte[] |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.Text;

    public class VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das VBA-Projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Daten für die Designer-Speicherung vorbereiten
            string storageName = "MyDesignerStorage";
            byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
            
            try
            {
                // AddDesignerStorage-Methode aufrufen
                vbaProject.Modules.AddDesignerStorage(storageName, storageData);
                
                Console.WriteLine("Designer storage added successfully");
                
                // Überprüfen, ob die Speicherung hinzugefügt wurde
                byte[] retrievedData = vbaProject.Modules.GetDesignerStorage(storageName);
                if (retrievedData != null)
                {
                    Console.WriteLine("Retrieved storage data: " + Encoding.UTF8.GetString(retrievedData));
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddDesignerStorage method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


