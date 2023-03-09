---
title: WorkbookMetadata classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata classe
Représente les métadonnées.



Le type WorkbookMetadata expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Créez l'objet de métadonnées.|
| [WorkbookMetadata(stream, options)](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Créez l'objet de métadonnées.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [options](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/options) | Obtient les options des métadonnées.|
| [built_in_document_properties](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul.|
| [custom_document_properties](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [save(file_name)](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Enregistrez les métadonnées modifiées dans le fichier.|
| [save(stream)](/cells/fr/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Enregistrez les métadonnées modifiées dans le flux.|



###  Exemple

L'exemple suivant crée un WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Voir également
* module [aspose.cells.metadata](..)
* classe [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty)
