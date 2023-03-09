---
title: classe VbaProject
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
##  classe VbaProject
Rappresenta il progetto VBA.



Il tipo VbaProject espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [is_valid_signed](/cells/it/python-net/aspose.cells.vba/vbaproject/is_valid_signed) | Indica se la firma del progetto VBA è valida o meno.|
| [cert_raw_data](/cells/it/python-net/aspose.cells.vba/vbaproject/cert_raw_data) | Ottiene i dati non elaborati del certificato se questo progetto VBA è firmato.|
| [name](/cells/it/python-net/aspose.cells.vba/vbaproject/name) | Ottiene e imposta il nome del progetto VBA.|
| [is_signed](/cells/it/python-net/aspose.cells.vba/vbaproject/is_signed) | Indica se VBAcode è firmato o meno.|
| [is_protected](/cells/it/python-net/aspose.cells.vba/vbaproject/is_protected) | Indica se questo progetto VBA è protetto.|
| [islocked_for_viewing](/cells/it/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) | Indica se questo progetto VBA è bloccato per la visualizzazione.|
| [modules](/cells/it/python-net/aspose.cells.vba/vbaproject/modules) | Ottiene tutti gli oggetti [VbaModule](/cells/it/python-net/aspose.cells.vba/vbamodule).|
| [references](/cells/it/python-net/aspose.cells.vba/vbaproject/references) | Ottiene tutti i riferimenti del progetto VBA.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [sign(digital_signature)](/cells/it/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) | Firma questo progetto VBA con una firma digitale|
| [protect(islocked_for_viewing, password)](/cells/it/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) | Protegge o rimuove la protezione di questo progetto VBA.|
| [copy(source)](/cells/it/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) | Copia il progetto VBA da un altro file.|
| [validate_password(password)](/cells/it/python-net/aspose.cells.vba/vbaproject/validate_password/#str) | Convalida la password di protezione.|



###  Esempi

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Guarda anche
* modulo [aspose.cells.vba](..)
* classe [VbaModule](/cells/it/python-net/aspose.cells.vba/vbamodule)
