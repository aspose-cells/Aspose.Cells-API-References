---
title: "CoWorkUserProvider"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Benutzer‑Provider‑Schnittstelle im Kollaborationsmodus dar. Nur in der Java‑Version verfügbar, wird in Zukunft in der .netython‑Version verfügbar sein."
type: docs
url: /de/java/com.aspose.gridjs/coworkuserprovider/
---
```
public interface CoWorkUserProvider
```

Stellt die Benutzeranbieter‑Schnittstelle im Kollaborationsmodus dar. Nur in der Java‑Version verfügbar, wird in Zukunft in .net/python‑Versionen verfügbar sein. Kundenanwendungen können diese Schnittstelle implementieren, um Benutzerinformationen bereitzustellen.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCurrentUserId()](#getCurrentUserId--) | Ermittelt die eindeutige Kennung des aktuellen Benutzers |
| [getCurrentUserName()](#getCurrentUserName--) | Ermittelt den Benutzernamen des aktuellen Benutzers |
| [getPermission()](#getPermission--) | Ermittelt die Berechtigungsstufe des aktuellen Benutzers |
### getCurrentUserId() {#getCurrentUserId--}
```
public abstract long getCurrentUserId()
```


Ermittelt die eindeutige Kennung des aktuellen Benutzers

**Returns:**
long - Aktuelle Benutzer‑ID
### getCurrentUserName() {#getCurrentUserName--}
```
public abstract String getCurrentUserName()
```


Ermittelt den Benutzernamen des aktuellen Benutzers

**Returns:**
java.lang.String - Aktueller Benutzername
### getPermission() {#getPermission--}
```
public abstract int getPermission()
```


Ermittelt die Berechtigungsstufe des aktuellen Benutzers

**Returns:**
int - [CoWorkUserPermission](../../com.aspose.gridjs/coworkuserpermission). Aktuelle Berechtigungsstufe des Benutzers
