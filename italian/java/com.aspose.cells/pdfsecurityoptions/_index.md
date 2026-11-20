---
title: "PdfSecurityOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni per la crittografia e le autorizzazioni di accesso per un documento PDF."
type: docs
url: /it/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Opzioni per la crittografia e i permessi di accesso di un documento PDF. PDF/A non consente impostazioni di sicurezza.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | Il costruttore di PdfSecurityOptions |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Indica se consentire l'assemblaggio del documento (inserimento, rotazione o eliminazione di pagine e creazione di segnalibri o miniature), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Indica se consentire la copia o l'estrazione di testo e grafica dal documento mediante operazioni diverse da quelle controllate da [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Permesso di copiare o estrarre contenuto obsoleto secondo la specifica PDF. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Indica se consentire la compilazione di campi di modulo interattivi esistenti (inclusi i campi firma), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Indica se consentire la stampa del documento in una rappresentazione da cui può essere generata una copia digitale fedele del contenuto PDF. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Indica se consentire la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) e [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Restituisce la password del proprietario per il documento PDF crittografato. |
| [getPrintPermission()](#getPrintPermission--) | Indica se consentire la stampa del documento. |
| [getUserPassword()](#getUserPassword--) | Restituisce la password utente necessaria per aprire il documento PDF crittografato. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Indica se consentire l'assemblaggio del documento (inserimento, rotazione o eliminazione di pagine e creazione di segnalibri o miniature), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Indica se consentire la copia o l'estrazione di testo e grafica dal documento mediante operazioni diverse da quelle controllate da [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Permesso di copiare o estrarre contenuto obsoleto secondo la specifica PDF. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Indica se consentire la compilazione di campi di modulo interattivi esistenti (inclusi i campi firma), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Indica se consentire la stampa del documento in una rappresentazione da cui può essere generata una copia digitale fedele del contenuto PDF. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Indica se consentire la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) e [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Imposta la password del proprietario per il documento PDF crittografato. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Indica se consentire la stampa del documento. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Imposta la password utente necessaria per aprire il documento PDF crittografato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


Il costruttore di PdfSecurityOptions

**Example**

Il codice seguente imposta il permesso di stampa ad alta risoluzione per il PDF di output.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi.

**Remarks**

Se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è anche impostato, crea o modifica campi di modulo interattivi (inclusi i campi firma).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Indica se consentire l'assemblaggio del documento (inserimento, rotazione o eliminazione di pagine e creazione di segnalibri o miniature), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo.

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


Indica se consentire la copia o l'estrazione di testo e grafica dal documento mediante operazioni diverse da quelle controllate da [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Permesso di copiare o estrarre contenuto obsoleto secondo la specifica PDF.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ExtractContentPermission. Questa proprietà sarà rimossa 12 mesi dopo, a partire da settembre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Indica se consentire la compilazione di campi di modulo interattivi esistenti (inclusi i campi firma), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Indica se consentire la stampa del documento in una rappresentazione da cui può essere generata una copia digitale fedele del contenuto PDF.

**Remarks**

Quando è attivo (e [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) è impostato), la stampa è limitata a una rappresentazione di basso livello dell'aspetto, possibilmente di qualità degradata.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Indica se consentire la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) e [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Restituisce la password del proprietario per il documento PDF crittografato.

**Remarks**

La password del proprietario consente all'utente di aprire un documento PDF crittografato senza alcuna restrizione di accesso specificata.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Indica se consentire la stampa del documento.

**Remarks**

Potrebbe non essere al livello di massima qualità, a seconda che [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) sia anche impostato.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Restituisce la password utente necessaria per aprire il documento PDF crittografato.

**Remarks**

La password del proprietario o la password dell'utente saranno richieste per aprire un documento PDF crittografato per la visualizzazione.

La password dell'utente può essere null o una stringa vuota; in questo caso non sarà richiesta alcuna password all'utente durante l'apertura del documento PDF.

Aprire il documento con la password del proprietario corretta consente l'accesso completo al documento.

Aprire il documento con la password dell'utente corretta (o aprire un documento che non ha una password utente) consente un accesso limitato secondo le autorizzazioni specificate.

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


Indica se consentire l'estrazione di testo e grafica (a supporto dell'accessibilità per utenti con disabilità o per altri scopi).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Indica se consentire l'aggiunta o la modifica di annotazioni di testo, la compilazione di campi di modulo interattivi.

**Remarks**

Se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è anche impostato, crea o modifica campi di modulo interattivi (inclusi i campi firma).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Indica se consentire l'assemblaggio del documento (inserimento, rotazione o eliminazione di pagine e creazione di segnalibri o miniature), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Indica se consentire la copia o l'estrazione di testo e grafica dal documento mediante operazioni diverse da quelle controllate da [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Permesso di copiare o estrarre contenuto obsoleto secondo la specifica PDF.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ExtractContentPermission. Questa proprietà sarà rimossa 12 mesi dopo, a partire da settembre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Indica se consentire la compilazione di campi di modulo interattivi esistenti (inclusi i campi firma), anche se [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) è attivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Indica se consentire la stampa del documento in una rappresentazione da cui può essere generata una copia digitale fedele del contenuto PDF.

**Remarks**

Quando è attivo (e [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) è impostato), la stampa è limitata a una rappresentazione di basso livello dell'aspetto, possibilmente di qualità degradata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Indica se consentire la modifica del contenuto del documento mediante operazioni diverse da quelle controllate da [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) e [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Imposta la password del proprietario per il documento PDF crittografato.

**Remarks**

La password del proprietario consente all'utente di aprire un documento PDF crittografato senza alcuna restrizione di accesso specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Indica se consentire la stampa del documento.

**Remarks**

Potrebbe non essere al livello di massima qualità, a seconda che [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) sia anche impostato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Imposta la password utente necessaria per aprire il documento PDF crittografato.

**Remarks**

La password del proprietario o la password dell'utente saranno richieste per aprire un documento PDF crittografato per la visualizzazione.

La password dell'utente può essere null o una stringa vuota; in questo caso non sarà richiesta alcuna password all'utente durante l'apertura del documento PDF.

Aprire il documento con la password del proprietario corretta consente l'accesso completo al documento.

Aprire il documento con la password dell'utente corretta (o aprire un documento che non ha una password utente) consente un accesso limitato secondo le autorizzazioni specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

