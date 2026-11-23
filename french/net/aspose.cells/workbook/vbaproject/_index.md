---
title: "Workbook.VbaProject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient le VbaProject dans une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Obtient le `VbaProject` dans une feuille de calcul.

```csharp
public VbaProject VbaProject { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez au projet VBA (VbaProject est en lecture seule, nous ne pouvons que vérifier s'il existe)
            if (workbook.VbaProject == null)
            {
                // Créez un projet VBA en enregistrant sous forme de classeur avec macros activées
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Ajoutez un nouveau module au projet VBA
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Récupérez le module ajouté et définissez son code
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Enregistrez le classeur
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Voir aussi

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


