---
title: "PdfSecurityOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options de chiffrement et d'autorisations d'accès pour un document PDF."
type: docs
url: /fr/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Options de chiffrement et d'autorisations d'accès pour un document PDF. PDF/A ne permet pas les paramètres de sécurité.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | Le constructeur de PdfSecurityOptions |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Indique s'il faut autoriser l'extraction de texte et de graphiques (dans le cadre de l'accessibilité pour les utilisateurs en situation de handicap ou à d'autres fins). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | Autorisation de copier ou d'extraire du contenu obsolète selon la référence PDF. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Indique s'il faut autoriser le remplissage des champs de formulaire interactifs existants (y compris les champs de signature), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF peut être générée. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) et [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | Obtient le mot de passe propriétaire du document PDF chiffré. |
| [getPrintPermission()](#getPrintPermission--) | Indique s'il faut autoriser l'impression du document. |
| [getUserPassword()](#getUserPassword--) | Obtient le mot de passe utilisateur requis pour ouvrir le document PDF chiffré. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Indique s'il faut autoriser l'extraction de texte et de graphiques (dans le cadre de l'accessibilité pour les utilisateurs en situation de handicap ou à d'autres fins). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | Autorisation de copier ou d'extraire du contenu obsolète selon la référence PDF. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Indique s'il faut autoriser le remplissage des champs de formulaire interactifs existants (y compris les champs de signature), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF peut être générée. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) et [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Définit le mot de passe propriétaire du document PDF chiffré. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Indique s'il faut autoriser l'impression du document. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


Le constructeur de PdfSecurityOptions

**Example**

Le code suivant définit une autorisation d'impression haute résolution pour le PDF de sortie.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Indique s'il faut autoriser l'extraction de texte et de graphiques (dans le cadre de l'accessibilité pour les utilisateurs en situation de handicap ou à d'autres fins).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs.

**Remarks**

si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est également activé, créez ou modifiez des champs de formulaire interactifs (y compris les champs de signature).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé.

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


Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


Autorisation de copier ou d'extraire du contenu obsolète selon la référence PDF.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ExtractContentPermission. Cette propriété sera supprimée 12 mois plus tard, à compter de septembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Indique s'il faut autoriser le remplissage des champs de formulaire interactifs existants (y compris les champs de signature), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF peut être générée.

**Remarks**

Lorsqu'il est activé (et que [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) est défini), l'impression est limitée à une représentation de bas niveau de l'apparence, éventuellement de qualité dégradée.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) et [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Obtient le mot de passe propriétaire du document PDF chiffré.

**Remarks**

Le mot de passe propriétaire permet à l'utilisateur d'ouvrir un document PDF chiffré sans aucune restriction d'accès spécifiée.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Indique s'il faut autoriser l'impression du document.

**Remarks**

Possiblement pas au niveau de qualité le plus élevé, selon que [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) est également définie.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Obtient le mot de passe utilisateur requis pour ouvrir le document PDF chiffré.

**Remarks**

Le mot de passe du propriétaire ou le mot de passe de l'utilisateur sera requis pour ouvrir un document PDF chiffré en vue.

Le mot de passe de l'utilisateur peut être nul ou une chaîne vide, dans ce cas aucun mot de passe ne sera demandé à l'utilisateur lors de l'ouverture du document PDF.

Ouvrir le document avec le mot de passe du propriétaire correct permet un accès complet au document.

Ouvrir le document avec le mot de passe de l'utilisateur correct (ou ouvrir un document qui n'a pas de mot de passe d'utilisateur) permet un accès limité selon les autorisations spécifiées.

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


Indique s'il faut autoriser l'extraction de texte et de graphiques (dans le cadre de l'accessibilité pour les utilisateurs en situation de handicap ou à d'autres fins).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Indique s'il faut autoriser l'ajout ou la modification d'annotations de texte, le remplissage de champs de formulaire interactifs.

**Remarks**

si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est également activé, créez ou modifiez des champs de formulaire interactifs (y compris les champs de signature).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Indique s'il faut autoriser l'assemblage du document (insertion, rotation ou suppression de pages et création de signets ou d'images miniatures), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Indique s'il faut autoriser la copie ou l'extraction de texte et de graphiques du document par des opérations autres que celles contrôlées par [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


Autorisation de copier ou d'extraire du contenu obsolète selon la référence PDF.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ExtractContentPermission. Cette propriété sera supprimée 12 mois plus tard, à compter de septembre 2023. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Indique s'il faut autoriser le remplissage des champs de formulaire interactifs existants (y compris les champs de signature), même si [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) est activé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


Indique s'il faut autoriser l'impression du document vers une représentation à partir de laquelle une copie numérique fidèle du contenu PDF peut être générée.

**Remarks**

Lorsqu'il est activé (et que [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) est défini), l'impression est limitée à une représentation de bas niveau de l'apparence, éventuellement de qualité dégradée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Indique s'il faut autoriser la modification du contenu du document par des opérations autres que celles contrôlées par [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) et [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Définit le mot de passe propriétaire du document PDF chiffré.

**Remarks**

Le mot de passe propriétaire permet à l'utilisateur d'ouvrir un document PDF chiffré sans aucune restriction d'accès spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Indique s'il faut autoriser l'impression du document.

**Remarks**

Possiblement pas au niveau de qualité le plus élevé, selon que [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) est également définie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Définit le mot de passe utilisateur requis pour ouvrir le document PDF chiffré.

**Remarks**

Le mot de passe du propriétaire ou le mot de passe de l'utilisateur sera requis pour ouvrir un document PDF chiffré en vue.

Le mot de passe de l'utilisateur peut être nul ou une chaîne vide, dans ce cas aucun mot de passe ne sera demandé à l'utilisateur lors de l'ouverture du document PDF.

Ouvrir le document avec le mot de passe du propriétaire correct permet un accès complet au document.

Ouvrir le document avec le mot de passe de l'utilisateur correct (ou ouvrir un document qui n'a pas de mot de passe d'utilisateur) permet un accès limité selon les autorisations spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

