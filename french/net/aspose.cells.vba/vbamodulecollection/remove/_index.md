---
title: "VbaModuleCollection.Remove"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaModuleCollection. Supprime le module d'une feuille de calcul"
type: docs
url: /fr/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Supprime le module d'une feuille de calcul.

```csharp
public void Remove(Worksheet sheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| feuille | Feuille de calcul | La feuille de calcul |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un module VBA à la feuille de calcul
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Obtenir la collection de modules VBA
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Appeler la méthode Remove avec le paramètre de la feuille de calcul
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Vérifier que le module a été supprimé
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Enregistrer le résultat
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Supprimer le module par le nom

```csharp
public void Remove(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String |  |

### Exemples

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
            // Créer un classeur avec macro
            Workbook workbook = new Workbook();
            
            // Accéder au projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter un nouveau module
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Ajouter du code au module
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Enregistrez le classeur
            workbook.Save("output_with_module.xlsm");
            
            // Supprimer le module par son nom
            vbaProject.Modules.Remove("TestModule");
            
            // Enregistrer le classeur après la suppression
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


