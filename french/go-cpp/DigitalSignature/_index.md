---
title: "DigitalSignature Classe"
linktitle: "DigitalSignature"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "DigitalSignature classe. Encapsule l'objet qui représente la signature numérique dans Go."
type: docs
weight: 200
url: /fr/go-cpp/digitalsignature/
---

## DigitalSignature class

Signature dans le fichier.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | Constructeur de DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | Constructeur de DigitalSignature. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetComments](./getcomments/) | Le but de la signature. |
| [SetComments](./setcomments/) | Le but de la signature. |
| [GetSignTime](./getsigntime/) | Le moment où le document a été signé. |
| [SetSignTime](./setsigntime/) | Le moment où le document a été signé. |
| [GetId](./getid/) | Spécifie un GUID qui peut être référencé croisé avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Vide (tous les zéros) GUID. |
| [SetId](./setid/) | Spécifie un GUID qui peut être référencé croisé avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Vide (tous les zéros) GUID. |
| [GetText](./gettext/) | Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Vide. |
| [SetText](./settext/) | Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Vide. |
| [GetImage](./getimage/) | Spécifie une image pour la signature numérique. La valeur par défaut est null. |
| [SetImage](./setimage/) | Spécifie une image pour la signature numérique. La valeur par défaut est null. |
| [GetProviderId](./getproviderid/) | Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Vide (tous les zéros) GUID. |
| [SetProviderId](./setproviderid/) | Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Vide (tous les zéros) GUID. |
| [IsValid](./isvalid/) | Si cette signature numérique est valide et que le document n'a pas été altéré, cette valeur sera vraie. |
| [GetXAdESType](./getxadestype/) | Type XAdES. La valeur par défaut est Aucun (XAdES est désactivé). |
| [SetXAdESType](./setxadestype/) | Type XAdES. La valeur par défaut est Aucun (XAdES est désactivé). |
