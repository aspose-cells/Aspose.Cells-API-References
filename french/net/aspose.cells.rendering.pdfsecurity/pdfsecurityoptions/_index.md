---
title: "Class PdfSecurityOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions class. Options de chiffrement et d'autorisations d'accès pour un document PDF. PDF/A ne permet pas les paramètres de sécurité."
type: docs
url: /fr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Options de chiffrement et d'autorisations d'accès pour un document PDF. PDF/A ne permet pas les paramètres de sécurité.

```csharp
public class PdfSecurityOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | Le constructeur de PdfSecurityOptions |

## Propriétés

| Nom | Description |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Indique s'il faut autoriser l'extraction de texte et de graphiques (pour soutenir l'accessibilité des utilisateurs handicapés ou à d'autres fins). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [`ModifyDocumentPermission`](./modifydocumentpermission/) est activé. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolète.**) Permission de copier ou d'extraire du contenu Obsolète selon la référence PDF. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Indique s'il faut autoriser le remplissage des champs de formulaire interactifs existants (y compris les champs de signature), même si [`ModifyDocumentPermission`](./modifydocumentpermission/) est activé. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF pourrait être générée. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) et [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Obtient ou définit le mot de passe propriétaire du document PDF chiffré. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Indique s'il faut autoriser l'impression du document. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Obtient ou définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Créer PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Créer PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Définir les options de sécurité
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // Attribuer des options de sécurité à PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Enregistrer le classeur en PDF avec les options de sécurité spécifiées
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


