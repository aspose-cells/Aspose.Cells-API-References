---
title: "SpreadsheetLocker"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "API low‑code pour verrouiller le fichier de feuille de calcul."
type: docs
url: /fr/java/com.aspose.cells/spreadsheetlocker/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetLocker
```

API low‑code pour verrouiller le fichier de feuille de calcul.

**Example**

```
         SpreadsheetLocker.process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| [process(String templateFile, String resultFile, String openPassword, String writePassword)](#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeProtectionProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeProtectionProvider provider)
```


Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Options d'entrée et de chargement |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Options de sortie et d'enregistrement |
| provider | [AbstractLowCodeProtectionProvider](../../com.aspose.cells/abstractlowcodeprotectionprovider) | Implémentation pour fournir les paramètres de protection |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword)
```


Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Options d'entrée et de chargement |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Options de sortie et d'enregistrement |
| openPassword | java.lang.String | Mot de passe pour le chiffrement du fichier |
| writePassword | java.lang.String | Mot de passe pour la protection de la modification de la feuille de calcul |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-java.lang.String-java.lang.String-java.lang.String-int-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, String openPassword, String writePassword, String workbookPassword, int workbookType)
```


Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Options d'entrée et de chargement |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Options de sortie et d'enregistrement |
| openPassword | java.lang.String | Mot de passe pour le chiffrement du fichier |
| writePassword | java.lang.String | Mot de passe pour la protection de la modification de la feuille de calcul |
| workbookPassword | java.lang.String | Mot de passe pour la protection du classeur |
| workbookType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection pour protéger le classeur |

### process(String templateFile, String resultFile, String openPassword, String writePassword) {#process-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile, String openPassword, String writePassword)
```


Verrouille le fichier de feuille de calcul avec les paramètres spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | java.lang.String | Le fichier modèle à verrouiller |
| resultFile | java.lang.String | Le fichier résultant |
| openPassword | java.lang.String | Mot de passe pour le chiffrement du fichier |
| writePassword | java.lang.String | Mot de passe pour la protection de la modification de la feuille de calcul |

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

