---
title: "VbaModule.BinaryCodes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété VbaModule. Obtient et définit les codes binaires du module"
type: docs
url: /fr/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Obtient et définit les codes binaires du module.

```csharp
public byte[] BinaryCodes { get; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // Chargez le classeur avec le projet VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Accéder au projet VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Obtenez les codes binaires du premier module
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Convertissez en chaîne en utilisant l'encodage chinois (936)
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Affichez le contenu contenant des caractères chinois
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Voir aussi

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


