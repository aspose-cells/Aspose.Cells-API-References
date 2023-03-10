---
title: provider_id proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells.digitalsignatures/digitalsignature/provider_id/
is_root: false
---
##  provider_id proprietà

Specifica l'ID classe del provider della firma.
Il valore predefinito è Guid vuoto (tutti zeri).

###  Osservazioni

Il provider di servizi di crittografia (CSP) è un modulo software indipendente che esegue effettivamente algoritmi di crittografia per l'autenticazione, la codifica e la crittografia.
Microsoft Office riserva il valore di {00000000-0000-0000-0000-000000000000} per il provider di firma predefinito,
e {000CD6A4-0000-0000-C000-000000000046} per il provider di firme dell'Asia orientale.

Il GUID del provider installato in aggiunta deve essere ottenuto dalla documentazione fornita con il provider.
###  Definizione:
```python
@property
def provider_id(self):
    ...
@provider_id.setter
def provider_id(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.digitalsignatures](../../)
* classe [DigitalSignature](/cells/it/python-net/aspose.cells.digitalsignatures/digitalsignature)
