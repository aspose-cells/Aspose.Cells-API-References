---
title: provider_id Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
##  provider_id Eigentum

Gibt die Klassen-ID des Signaturanbieters an.
Der Standardwert ist leer (nur Nullen) Guid.

###  Bemerkungen

Der Cryptographic Service Provider (CSP) ist ein unabhängiges Softwaremodul, das tatsächlich Kryptographiealgorithmen zur Authentifizierung, Kodierung und Verschlüsselung ausführt.
Microsoft Office reserviert den Wert {00000000-0000-0000-0000-000000000000} für seinen Standard-Signaturanbieter,
und {000CD6A4-0000-0000-C000-000000000046} für seinen ostasiatischen Signaturanbieter.

Die GUID des zusätzlich installierten Providers entnehmen Sie bitte der mitgelieferten Dokumentation des Providers.
###  Definition:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.digitalsignatures](../../)
* Klasse [DigitalSignature](/cells/de/python-net/aspose.cells.digitalsignatures/digitalsignature)
