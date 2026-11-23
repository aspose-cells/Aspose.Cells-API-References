---
title: "Classe VbaProject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Vba.VbaProject. Représente le projet VBA"
type: docs
url: /fr/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

Représente le projet VBA.

```csharp
public class VbaProject
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Obtient les données brutes du certificat si ce projet VBA est signé. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | Obtient et définit l'encodage du projet VBA. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Indique si ce projet VBA est verrouillé pour la visualisation. Si vrai, le code ne peut pas être visible. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolète.**) Indique si ce projet VBA est verrouillé pour la visualisation. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Indique si ce projet VBA est protégé. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | Indique si le code VBA est signé ou non. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | Indique si la signature du projet VBA est valide ou non. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Récupère tous les objets [`VbaModule`](../vbamodule/). |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | Obtient et définit le nom du projet VBA. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | Récupère toutes les références du projet VBA. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | Copie le projet VBA depuis un autre fichier. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Protège ou déprotège ce projet VBA. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Signe ce projet VBA avec une DigitalSignature |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Valide le mot de passe de protection. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Text;
    using System.Security.Cryptography.X509Certificates;

    public class VbaProjectDemo
    {
        public static void VbaProjectExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Initialiser le projet VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Définition des propriétés
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Vérification des propriétés en lecture seule
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Ajout d'un module VBA
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Ajout d'une référence de projet VBA
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Protection du projet VBA
            vbaProject.Protect(true, "password");

            // Signature du projet VBA
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Enregistrement du fichier Excel
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


