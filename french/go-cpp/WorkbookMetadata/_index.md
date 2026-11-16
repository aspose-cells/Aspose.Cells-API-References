---
title: "Classe WorkbookMetadata"
linktitle: "WorkbookMetadata"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe WorkbookMetadata. Encapsule l'objet qui représente workbookmetadata en Go."
type: docs
weight: 200
url: /fr/go-cpp/workbookmetadata/
---

## WorkbookMetadata class

Représente les métadonnées.

```go

type WorkbookMetadata struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |
| [NewWorkbookMetadata_String_MetadataOptions](./newworkbookmetadata_string_metadataoptions/) | Crée l'objet de métadonnées. |
| [NewWorkbookMetadata_Stream_MetadataOptions](./newworkbookmetadata_stream_metadataoptions/) | Crée l'objet de métadonnées. |

## Méthodes

| Méthode | Description |
| --- | --- |
| [IsNull](./isnull/) | Vérifie si l'objet d'implémentation est nullptr. |
| [GetOptions](./getoptions/) | Obtient les options des métadonnées. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Renvoie une collection DocumentProperty qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [Save_String](./save_string/) | Enregistre les métadonnées modifiées dans le fichier. |
| [Save_Stream](./save_stream/) | Enregistre les métadonnées modifiées dans le flux. |
