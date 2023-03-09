---
title: ReConnectionMethodType enumerazione
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 130
url: /it/python-net/aspose.cells.externalconnections/reconnectionmethodtype/
is_root: false
---
##  ReConnectionMethodType enumerazione
Specifica cosa deve fare l'applicazione del foglio di calcolo quando una connessione fallisce.



Il tipo ReConnectionMethodType espone i membri seguenti:

###  Campi
| Campo| Descrizione|
| :- | :- |
| REQUIRED | All'aggiornamento utilizzare le informazioni di connessione esistenti e se finiscono per non essere valide<br/> quindi ottenere le informazioni di connessione aggiornate, se disponibili dal file di connessione esterno.|
| ALWAYS | Ad ogni aggiornamento ottenere informazioni di connessione aggiornate dal file di connessione esterno,<br/> se disponibile, e usalo al posto delle informazioni di connessione esistenti.<br/> In questo caso l'aggiornamento dei dati fallirà se il file di connessione esterno non è disponibile.|
| NEVER | Non ottenere mai informazioni di connessione aggiornate dal file di connessione esterno<br/> anche se è disponibile e anche se le informazioni sulla connessione esistente non sono valide|



###  Guarda anche
* modulo [aspose.cells.externalconnections](..)
