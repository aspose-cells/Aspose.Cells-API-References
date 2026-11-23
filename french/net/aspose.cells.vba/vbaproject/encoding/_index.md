---
title: "VbaProject.Encoding"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaProject. Obtient et définit le codage du projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

Obtient et définit l'encodage du projet VBA.

```csharp
public Encoding Encoding { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Définir les propriétés du projet VBA incluant le codage
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Ajouter un module au projet VBA
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // Enregistrer le classeur avec le projet VBA
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


