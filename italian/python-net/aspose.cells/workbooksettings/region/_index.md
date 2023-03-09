---
title: region proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 520
url: /it/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
##  region proprietà

Ottiene o imposta le impostazioni internazionali per la cartella di lavoro.

###  Osservazioni

1. Impostazioni internazionali utilizzate dal componente Aspose.Cells per una cartella di lavoro caricata dal file modello:
io). Per un file XLS, sono presenti campi definiti per le impostazioni internazionali e MS Excel salva i dati delle impostazioni regionali nel file quando si salva il file XLS.
Quindi, usiamo lo region salvato nel file modello per la cartella di lavoro.
Se non si desidera utilizzare lo region salvato nel file XLS, reimpostarlo su quello previsto (ad esempio CountryCode.Default) dopo aver caricato il file modello.
Inoltre, salviamo anche il valore specificato dall'utente (con questo metodo) nel file quando salviamo un file XLS.
ii). Per altri formati di file, come XLSX, XLSB...ecc., non esiste alcun campo definito per le impostazioni internazionali nella specifica del formato di file.
Quindi, utilizziamo le impostazioni regionali dell'ambiente dell'applicazione per la cartella di lavoro.
Inoltre, il valore specificato dall'utente (con questo metodo) non può essere mantenuto per i file generati con quei formati di file.
2. Per l'effetto vista in MS Excel:
Le impostazioni regionali applicate qui possono avere effetto solo in fase di esecuzione con il componente Aspose.Cells e non durante la visualizzazione del file generato con MS Excel.
Anche per il file XLS generato in cui sono stati salvati i dati delle impostazioni internazionali specificati, durante la visualizzazione/modifica con MS Excel,
lo region utilizzato per eseguire la formattazione da MS Excel è sempre l'impostazione regionale predefinita dell'ambiente in cui è in esecuzione MS Excel,
non quello salvato nel file. È il comportamento di MS Excel e non può essere modificato dal codice.
###  Definizione:
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [CountryCode](/cells/it/python-net/aspose.cells/countrycode)
* classe [WorkbookSettings](/cells/it/python-net/aspose.cells/workbooksettings)
