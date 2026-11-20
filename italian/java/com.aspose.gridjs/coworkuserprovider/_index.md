---
title: "CoWorkUserProvider"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia del provider utente in modalità collaborazione. Disponibile solo nella versione Java al momento, sarà disponibile nella versione .netython in futuro."
type: docs
url: /it/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Rappresenta l'interfaccia del provider utente in modalità collaborazione. Disponibile solo nella versione Java al momento, sarà disponibile nella versione .net/python in futuro. L'applicazione cliente può implementare questa interfaccia per fornire le informazioni sull'utente.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Ottiene l'identificatore univoco dell'utente corrente |
| [getCurrentUserName()](#getCurrentUserName--) | Ottiene il nome utente dell'utente corrente |
| [getPermission()](#getPermission--) | Ottiene il livello di autorizzazione dell'utente corrente |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Ottiene l'identificatore univoco dell'utente corrente

**Returns:**
long - ID utente corrente
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Ottiene il nome utente dell'utente corrente

**Returns:**
java.lang.String - Nome utente corrente
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Ottiene il livello di autorizzazione dell'utente corrente

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Livello di autorizzazione dell'utente corrente
