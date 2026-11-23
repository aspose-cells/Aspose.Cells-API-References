---
title: "VbaModuleCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaModuleCollection. Obtient VbaModule dans la liste par l'index"
type: docs
url: /fr/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Obtient [`VbaModule`](../../vbamodule/) dans la liste par l'index.

```csharp
public VbaModule this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

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
            // Créer un nouveau classeur avec le projet VBA
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Obtenir le projet VBA existant (VbaProject est en lecture seule)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Ajouter un module au projet VBA
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Accéder au module en utilisant la propriété Item
            VbaModule module = vbaProject.Modules[index];
            
            // Ajouter du code VBA au module
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Enregistrez le classeur
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Voir aussi

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Obtient [`VbaModule`](../../vbamodule/) dans la liste par le nom.

```csharp
public VbaModule this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom du module. |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un module VBA au classeur
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Accéder au module en utilisant la propriété Item par nom
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // Définir le code VBA
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Enregistrez le classeur
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Vérifier en rechargeant
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Voir aussi

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


