---
title: "FileFormatInfo Classe"
linktitle: "FileFormatInfo"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe FileFormatInfo. Encapsule l'objet qui représente fileformatinfo en Go."
type: docs
weight: 200
url: /fr/go-cpp/fileformatinfo/
---

## FileFormatInfo class

Contient les données renvoyées par les méthodes de détection du format de fichier <see cref="FileFormatUtil"/>.

```go

type FileFormatInfo struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewFileFormatInfo](./newfileformatinfo/) | Constructeur par défaut. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [IsProtectedByRMS](./isprotectedbyrms/) | Indique si le fichier est protégé par Microsoft Rights Management Server. |
| [IsEncrypted](./isencrypted/) | Renvoie vrai si le document est chiffré et nécessite un mot de passe pour l'ouvrir. |
| [GetFileFormatType](./getfileformattype/) | Obtient le format de fichier détecté. |
| [GetLoadFormat](./getloadformat/) | Obtient le format de chargement détecté. |
