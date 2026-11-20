---
title: "PdfSecurityOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Optionen zum Verschlüsseln und für Zugriffsberechtigungen für ein PDF-Dokument."
type: docs
url: /de/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Optionen zum Verschlüsseln und für Zugriffsberechtigungen eines PDF-Dokuments. PDF/A erlaubt keine Sicherheitseinstellungen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | Der Konstruktor von PdfSecurityOptions |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) gesteuerten erlaubt ist. |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Erlaubnis zum Kopieren oder Extrahieren von Inhalten, laut PDF-Referenz veraltet. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Gibt an, ob das Drucken des Dokuments zu einer Darstellung erlaubt ist, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) und [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) gesteuerten erlaubt ist. |
| [getOwnerPassword()](#getOwnerPassword--) | Liest das Besitzerpasswort des verschlüsselten PDF-Dokuments. |
| [getPrintPermission()](#getPrintPermission--) | Gibt an, ob das Drucken des Dokuments erlaubt ist. |
| [getUserPassword()](#getUserPassword--) | Liest das Benutzerpasswort, das zum Öffnen des verschlüsselten PDF-Dokuments benötigt wird. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) gesteuerten erlaubt ist. |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Erlaubnis zum Kopieren oder Extrahieren von Inhalten, laut PDF-Referenz veraltet. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Gibt an, ob das Drucken des Dokuments zu einer Darstellung erlaubt ist, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) und [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) gesteuerten erlaubt ist. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Setzt das Besitzerpasswort für das verschlüsselte PDF-Dokument. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Gibt an, ob das Drucken des Dokuments erlaubt ist. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Legt das Benutzerpasswort fest, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


Der Konstruktor von PdfSecurityOptions

**Example**

Der folgende Code legt die hochauflösende Druckberechtigung für das Ausgabepdf fest.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist.

**Remarks**

wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) ebenfalls gesetzt ist, interaktive Formularfelder (einschließlich Signaturfelder) erstellen oder ändern.

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) gesteuerten erlaubt ist.

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Erlaubnis zum Kopieren oder Extrahieren von Inhalten, laut PDF-Referenz veraltet.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExtractContentPermission. Diese Eigenschaft wird 12 Monate später, seit September 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Gibt an, ob das Drucken des Dokuments zu einer Darstellung erlaubt ist, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann.

**Remarks**

Wenn es klar ist (und [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) gesetzt ist), ist das Drucken auf eine niedrigstufige Darstellung des Erscheinungsbildes beschränkt, möglicherweise von verminderter Qualität.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) und [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) gesteuerten erlaubt ist.

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Liest das Besitzerpasswort des verschlüsselten PDF-Dokuments.

**Remarks**

Das Besitzerpasswort ermöglicht dem Benutzer, ein verschlüsseltes PDF-Dokument zu öffnen, ohne dass Zugriffsrestriktionen festgelegt sind.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Gibt an, ob das Drucken des Dokuments erlaubt ist.

**Remarks**

Möglicherweise nicht auf höchster Qualitätsstufe, abhängig davon, ob [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) ebenfalls gesetzt ist.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Liest das Benutzerpasswort, das zum Öffnen des verschlüsselten PDF-Dokuments benötigt wird.

**Remarks**

Das Besitzerpasswort oder das Benutzerpasswort wird erforderlich sein, um ein verschlüsseltes PDF-Dokument zur Ansicht zu öffnen.

Das Benutzerpasswort kann null oder ein leerer String sein; in diesem Fall wird beim Öffnen des PDF-Dokuments kein Passwort vom Benutzer verlangt.

Das Öffnen des Dokuments mit dem korrekten Besitzerpasswort ermöglicht vollen Zugriff auf das Dokument.

Das Öffnen des Dokuments mit dem korrekten Benutzerpasswort (oder das Öffnen eines Dokuments, das kein Benutzerpasswort hat) ermöglicht eingeschränkten Zugriff gemäß den angegebenen Berechtigungen.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


Gibt an, ob das Extrahieren von Text und Grafiken erlaubt ist (zur Unterstützung der Barrierefreiheit für Benutzer mit Behinderungen oder zu anderen Zwecken).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Gibt an, ob das Hinzufügen oder Ändern von Textanmerkungen sowie das Ausfüllen interaktiver Formularfelder erlaubt ist.

**Remarks**

wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) ebenfalls gesetzt ist, interaktive Formularfelder (einschließlich Signaturfelder) erstellen oder ändern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Gibt an, ob das Zusammenstellen des Dokuments (Einfügen, Drehen oder Löschen von Seiten und Erstellen von Lesezeichen oder Miniaturbildern) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Gibt an, ob das Kopieren oder anderweitige Extrahieren von Text und Grafiken aus dem Dokument durch andere Vorgänge als die von [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) gesteuerten erlaubt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Erlaubnis zum Kopieren oder Extrahieren von Inhalten, laut PDF-Referenz veraltet.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft ExtractContentPermission. Diese Eigenschaft wird 12 Monate später, seit September 2023, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Gibt an, ob das Ausfüllen vorhandener interaktiver Formularfelder (einschließlich Signaturfelder) erlaubt ist, selbst wenn [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) deaktiviert ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Gibt an, ob das Drucken des Dokuments zu einer Darstellung erlaubt ist, aus der eine getreue digitale Kopie des PDF-Inhalts erzeugt werden kann.

**Remarks**

Wenn es klar ist (und [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) gesetzt ist), ist das Drucken auf eine niedrigstufige Darstellung des Erscheinungsbildes beschränkt, möglicherweise von verminderter Qualität.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Gibt an, ob das Ändern des Inhalts des Dokuments durch andere Vorgänge als die von [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) und [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) gesteuerten erlaubt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Setzt das Besitzerpasswort für das verschlüsselte PDF-Dokument.

**Remarks**

Das Besitzerpasswort ermöglicht dem Benutzer, ein verschlüsseltes PDF-Dokument zu öffnen, ohne dass Zugriffsrestriktionen festgelegt sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Gibt an, ob das Drucken des Dokuments erlaubt ist.

**Remarks**

Möglicherweise nicht auf höchster Qualitätsstufe, abhängig davon, ob [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) ebenfalls gesetzt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Legt das Benutzerpasswort fest, das zum Öffnen des verschlüsselten PDF-Dokuments erforderlich ist.

**Remarks**

Das Besitzerpasswort oder das Benutzerpasswort wird erforderlich sein, um ein verschlüsseltes PDF-Dokument zur Ansicht zu öffnen.

Das Benutzerpasswort kann null oder ein leerer String sein; in diesem Fall wird beim Öffnen des PDF-Dokuments kein Passwort vom Benutzer verlangt.

Das Öffnen des Dokuments mit dem korrekten Besitzerpasswort ermöglicht vollen Zugriff auf das Dokument.

Das Öffnen des Dokuments mit dem korrekten Benutzerpasswort (oder das Öffnen eines Dokuments, das kein Benutzerpasswort hat) ermöglicht eingeschränkten Zugriff gemäß den angegebenen Berechtigungen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

