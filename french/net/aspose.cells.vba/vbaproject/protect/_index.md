---
title: "VbaProject.Protect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VbaProject. Protège ou désactive la protection de ce projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Protège ou déprotège ce projet VBA.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| islockedForViewing | Boolean | indique si le projet est verrouillé pour la visualisation. |
| mot de passe | String | Si la valeur est nulle, désactive la protection de ce projet VBA, sinon protège ce projet VBA. |

### Remarques

Si islockedForViewing est vrai, le mot de passe ne peut pas être nul.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Créer un classeur avec le projet VBA
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Voir aussi

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


