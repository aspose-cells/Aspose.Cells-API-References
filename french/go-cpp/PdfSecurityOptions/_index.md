---
title: "Classe PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe PdfSecurityOptions. Encapsule l'objet qui représente pdfsecurityoptions en Go."
type: docs
weight: 200
url: /fr/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Options de chiffrement et d'autorisations d'accès pour un document PDF. PDF/A ne permet pas les paramètres de sécurité.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | Le constructeur de PdfSecurityOptions |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetUserPassword](./getuserpassword/) | Obtient ou définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré. |
| [SetUserPassword](./setuserpassword/) | Obtient ou définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré. |
| [GetOwnerPassword](./getownerpassword/) | Obtient ou définit le mot de passe propriétaire pour le document PDF chiffré. |
| [SetOwnerPassword](./setownerpassword/) | Obtient ou définit le mot de passe propriétaire pour le document PDF chiffré. |
| [GetPrintPermission](./getprintpermission/) | Indique s'il est permis d'imprimer le document. |
| [SetPrintPermission](./setprintpermission/) | Indique s'il est permis d'imprimer le document. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | Indique s'il est permis de modifier le contenu du document par des opérations autres que celles contrôlées par AnnotationsPermission, FillFormsPermission et AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | Indique s'il est permis de modifier le contenu du document par des opérations autres que celles contrôlées par AnnotationsPermission, FillFormsPermission et AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | Indique s'il est permis d'ajouter ou de modifier des annotations de texte, de remplir les champs de formulaire interactifs. |
| [SetAnnotationsPermission](./setannotationspermission/) | Indique s'il est permis d'ajouter ou de modifier des annotations de texte, de remplir les champs de formulaire interactifs. |
| [GetFillFormsPermission](./getfillformspermission/) | Indique s'il est permis de remplir les champs de formulaire interactifs existants (y compris les champs de signature), même si ModifyDocumentPermission est autorisé. |
| [SetFillFormsPermission](./setfillformspermission/) | Indique s'il est permis de remplir les champs de formulaire interactifs existants (y compris les champs de signature), même si ModifyDocumentPermission est autorisé. |
| [GetExtractContentPermission](./getextractcontentpermission/) | Indique s'il est permis de copier ou d'extraire autrement le texte et les graphiques du document par des opérations autres que celles contrôlées par AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | Indique s'il est permis de copier ou d'extraire autrement le texte et les graphiques du document par des opérations autres que celles contrôlées par AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Indique s'il est permis d'extraire le texte et les graphiques (dans le cadre de l'accessibilité pour les utilisateurs handicapés ou à d'autres fins). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Indique s'il est permis d'extraire le texte et les graphiques (dans le cadre de l'accessibilité pour les utilisateurs handicapés ou à d'autres fins). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | Indique s'il est permis d'assembler le document (insérer, faire pivoter ou supprimer des pages et créer des signets ou des images miniatures), même si ModifyDocumentPermission est autorisé. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | Indique s'il est permis d'assembler le document (insérer, faire pivoter ou supprimer des pages et créer des signets ou des images miniatures), même si ModifyDocumentPermission est autorisé. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | Indique s'il est permis d'imprimer le document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF pourrait être générée. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | Indique s'il est permis d'imprimer le document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF pourrait être générée. |
