---
title: "VbaModuleCollection.AddDesignerStorage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-metod."
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/adddesignerstorage/
---
## VbaModuleCollection.AddDesignerStorage method

```csharp
public void AddDesignerStorage(string name, byte[] data)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String |  |
| data | Byte[] |  |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till VBA-projektet
            VbaProject vbaProject = workbook.VbaProject;
            
            // Förbered data för designerlagring
            string storageName = "MyDesignerStorage";
            byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
            
            try
            {
                // Anropa AddDesignerStorage-metoden
                vbaProject.Modules.AddDesignerStorage(storageName, storageData);
                
                Console.WriteLine("Designer storage added successfully");
                
                // Verifiera att lagringen har lagts till
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
            
            // Spara arbetsboken
            workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
        }
    }
}
```

### Se även

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


