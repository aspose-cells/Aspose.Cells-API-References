---
title: "Classe SignatureLine"
linktitle: "SignatureLine"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "SignatureLine classe. Encapsule l'objet qui représente signatureline en Go."
type: docs
weight: 200
url: /fr/go-cpp/signatureline/
---

## SignatureLine class

Représente la ligne de signature.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetId](./getid/) | Obtient ou définit l'identifiant de cette ligne de signature. |
| [SetId](./setid/) | Obtient ou définit l'identifiant de cette ligne de signature. |
| [GetProviderId](./getproviderid/) | Obtient ou définit l'ID du fournisseur de signature. |
| [SetProviderId](./setproviderid/) | Obtient ou définit l'ID du fournisseur de signature. |
| [GetSigner](./getsigner/) | Obtient ou définit le signataire. |
| [SetSigner](./setsigner/) | Obtient ou définit le signataire. |
| [GetTitle](./gettitle/) | Obtient ou définit le titre du chanteur. |
| [SetTitle](./settitle/) | Obtient ou définit le titre du chanteur. |
| [GetEmail](./getemail/) | Obtient ou définit l'e-mail du chanteur. |
| [SetEmail](./setemail/) | Obtient ou définit l'e-mail du chanteur. |
| [IsLine](./isline/) | Indique s'il s'agit d'une ligne de signature. |
| [SetIsLine](./setisline/) | Indique s'il s'agit d'une ligne de signature. |
| [GetAllowComments](./getallowcomments/) | Indique si des commentaires peuvent être joints. |
| [SetAllowComments](./setallowcomments/) | Indique si des commentaires peuvent être joints. |
| [GetShowSignedDate](./getshowsigneddate/) | Indique si la date de signature doit être affichée. |
| [SetShowSignedDate](./setshowsigneddate/) | Indique si la date de signature doit être affichée. |
| [GetInstructions](./getinstructions/) | Obtient ou définit le texte affiché à l'utilisateur lors de la signature. |
| [SetInstructions](./setinstructions/) | Obtient ou définit le texte affiché à l'utilisateur lors de la signature. |
| [GetSignatureLineType](./getsignaturelinetype/) | Obtient ou définit le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur correspondante de ProviderId est fixée à {0000000000-0000-0000-0000-0000000000}. Stamp - Lorsque la valeur est Stamp, la valeur correspondante de ProviderId est généralement {000CD6A4-0000-0000-C000-000000000046}. Custom - Lorsque la valeur est Custom, la valeur correspondante de ProviderId doit généralement être définie par l'utilisateur. Elle doit être obtenue à partir de la documentation fournie avec le fournisseur. |
| [SetSignatureLineType](./setsignaturelinetype/) | Obtient ou définit le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur correspondante de ProviderId est fixée à {0000000000-0000-0000-0000-0000000000}. Stamp - Lorsque la valeur est Stamp, la valeur correspondante de ProviderId est généralement {000CD6A4-0000-0000-C000-000000000046}. Custom - Lorsque la valeur est Custom, la valeur correspondante de ProviderId doit généralement être définie par l'utilisateur. Elle doit être obtenue à partir de la documentation fournie avec le fournisseur. |
