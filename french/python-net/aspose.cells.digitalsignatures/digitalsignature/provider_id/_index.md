---
title: provider_id propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
##  provider_id propriété

Spécifie l'ID de classe du fournisseur de signature.
La valeur par défaut est Empty (tous les zéros) Guid.

###  Remarques

Le fournisseur de services cryptographiques (CSP) est un module logiciel indépendant qui exécute en fait des algorithmes de cryptographie pour l'authentification, le codage et le cryptage.
Microsoft Office réserve la valeur de {00000000-0000-0000-0000-000000000000} pour son fournisseur de signature par défaut,
et {000CD6A4-0000-0000-C000-000000000046} pour son fournisseur de signatures d'Asie de l'Est.

Le GUID du fournisseur installé en plus doit être obtenu à partir de la documentation fournie avec le fournisseur.
###  Définition:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Voir également
* module [aspose.cells.digitalsignatures](../../)
* classe [DigitalSignature](/cells/fr/python-net/aspose.cells.digitalsignatures/digitalsignature)
