---
title: "VbaModuleCollection.AddDesignerStorage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo VbaModuleCollection."
type: docs
url: /it/net/aspose.cells.vba/vbamodulecollection/adddesignerstorage/
---
## VbaModuleCollection.AddDesignerStorage method

```csharp
public void AddDesignerStorage(string name, byte[] data)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String |  |
| dati | Byte[] |  |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al progetto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Prepara i dati per l'archiviazione del designer
            string storageName = "MyDesignerStorage";
            byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
            
            try
            {
                // Chiama il metodo AddDesignerStorage
                vbaProject.Modules.AddDesignerStorage(storageName, storageData);
                
                Console.WriteLine("Designer storage added successfully");
                
                // Verifica che l'archiviazione sia stata aggiunta
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
            
            // Salva la cartella di lavoro
            workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


