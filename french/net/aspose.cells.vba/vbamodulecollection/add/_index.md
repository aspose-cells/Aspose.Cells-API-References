---
title: "VbaModuleCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaModuleCollection. Ajoute un module pour une feuille de calcul"
type: docs
url: /fr/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Ajoute le module pour une feuille de calcul.

```csharp
public int Add(Worksheet sheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| feuille | Feuille de calcul | La feuille de calcul |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un module VBA associé à la feuille de calcul
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Ajouter du code VBA au module
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Enregistrer le classeur avec le projet VBA
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
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

## Add(VbaModuleType, string) {#add}

Ajoute le module.

```csharp
public int Add(VbaModuleType type, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | VbaModuleType | Le type de module. |
| name | String | Le nom du module. |

### Exemples

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

### Voir aussi

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


