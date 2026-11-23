---
title: "Classe License"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.License. Fournit des méthodes pour licencier le composant"
type: docs
url: /fr/net/aspose.cells/license/
---
## License class

Fournit des méthodes pour licencier le composant.

```csharp
public class License
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [License](license/)() | Initialise une nouvelle instance de cette classe. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Licence le composant. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Licence le composant. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Créer une instance de la classe License
            License license = new License();

            // Définir la licence en utilisant le nom d'un fichier de licence
            license.SetLicense("Aspose.Cells.NET.lic");

            // Sinon, définissez la licence en utilisant un flux
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Code supplémentaire pour démontrer l'utilisation des fonctionnalités d'Aspose.Cells sous licence
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Enregistrez le classeur pour vérifier que la licence est appliquée correctement
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


