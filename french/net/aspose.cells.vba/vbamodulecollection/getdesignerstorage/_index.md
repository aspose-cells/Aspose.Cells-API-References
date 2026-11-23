---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaModuleCollection. Représente les données du concepteur"
type: docs
url: /fr/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Représente les données du Concepteur.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Remarques

Nous ne supportons pas l'analyse de ceux-ci. Seulement pour la copie.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // Créer un classeur avec le projet VBA
            Workbook workbook = new Workbook();
            
            // Ajouter un module de concepteur
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Obtenir le stockage du concepteur (sera nul initialement)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Ajouter des données de stockage du concepteur
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Obtenir et afficher le stockage du concepteur
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Voir aussi

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


