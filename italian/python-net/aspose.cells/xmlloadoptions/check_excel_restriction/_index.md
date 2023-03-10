---
title: check_excel_restriction proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/xmlloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction proprietà

Se controllare la restrizione del file excel quando l'utente modifica gli oggetti relativi alle celle.
Ad esempio, Excel non consente di inserire un valore di stringa più lungo di 32K.
Quando inserisci un valore più lungo di 32K, ad esempio Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione.
Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che in seguito
puoi emettere il valore di stringa completo per altri formati di file come CSV.
Tuttavia, se hai impostato un tipo di valore non valido per il formato di file excel,
non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato.
###  Definizione:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [XmlLoadOptions](/cells/it/python-net/aspose.cells/xmlloadoptions)
