---
title: "CoWorkUserProvider"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar användar‑leverantörsgränssnittet i samarbetsläge. Endast tillgängligt i Java‑versionen nu, kommer att bli tillgängligt i .net/python‑versionen i framtiden."
type: docs
url: /sv/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Representerar användar‑leverantörsgränssnittet i samarbetsläge. Endast tillgängligt i Java‑versionen nu, kommer att bli tillgängligt i .net/python‑versionen i framtiden. Kundapplikationen kan implementera detta gränssnitt för att tillhandahålla användarinformation.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Hämtar den unika identifieraren för den aktuella användaren |
| [getCurrentUserName()](#getCurrentUserName--) | Hämtar användarnamnet för den aktuella användaren |
| [getPermission()](#getPermission--) | Hämtar behörighetsnivån för den aktuella användaren |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Hämtar den unika identifieraren för den aktuella användaren

**Returns:**
long - Aktuellt användar‑ID
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Hämtar användarnamnet för den aktuella användaren

**Returns:**
java.lang.String - Aktuellt användarnamn
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Hämtar behörighetsnivån för den aktuella användaren

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Aktuell användarbehörighetsnivå
