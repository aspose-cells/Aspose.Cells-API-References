---
title: "GridJsLogger"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Fournit un système de journalisation léger pour le serveur GridJs."
type: docs
url: /fr/java/com.aspose.gridjs/gridjslogger/
---

**Inheritance:**
java.lang.Object
```
public class GridJsLogger
```

Fournit un système de journalisation léger pour le serveur GridJs. Prend en charge la sortie console et fichier avec des niveaux de journalisation configurables. Le niveau par défaut est Aucun. Dans une version DEBUG, le niveau par défaut est Debug (affiche tous les messages). Prend en charge la rotation des fichiers de journal par jour/semaine/mois.
## Méthodes

| Méthode | Description |
| --- | --- |
| [closeLogFile()](#closeLogFile--) | Ferme l'écrivain du fichier de journal et désactive la sortie fichier. |
| [debug(String message)](#debug-java.lang.String-) | Enregistre un message de niveau debug. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [error(String message)](#error-java.lang.String-) | Enregistre un message de niveau erreur. |
| [getClass()](#getClass--) |  |
| [getEnableConsoleOutput()](#getEnableConsoleOutput--) | Obtient si les messages de journal doivent être affichés dans la console. |
| [getEnableFileOutput()](#getEnableFileOutput--) | Obtient si les messages de journal doivent être écrits dans un fichier. |
| [getLevel()](#getLevel--) | Obtient le niveau de journal minimum. |
| [getLogFilePath()](#getLogFilePath--) | Obtient le chemin actuel du fichier de journal, ou null s'il n'est pas défini. |
| [getMaxFileSize()](#getMaxFileSize--) | Obtient la taille maximale (en octets) d'un fichier de journal avant rotation. |
| [hashCode()](#hashCode--) |  |
| [info(String message)](#info-java.lang.String-) | Enregistre un message de niveau info. |
| [log(int level, String message)](#log-int-java.lang.String-) | Enregistre un message au niveau spécifié. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEnableConsoleOutput(boolean value)](#setEnableConsoleOutput-boolean-) | Définit si les messages de journal doivent être affichés dans la console. |
| [setEnableFileOutput(boolean value)](#setEnableFileOutput-boolean-) | Définit si les messages de journal doivent être écrits dans un fichier. |
| [setLevel(int value)](#setLevel-int-) | Définit le niveau de journal minimal. |
| [setLogDirectory(String directory)](#setLogDirectory-java.lang.String-) | Définit le répertoire de journal avec une stratégie de rotation quotidienne des fichiers et active la sortie vers le fichier. |
| [setLogDirectory(String directory, int rolling)](#setLogDirectory-java.lang.String-int-) | Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. |
| [setLogDirectory(String directory, int rolling, String filePrefix)](#setLogDirectory-java.lang.String-int-java.lang.String-) | Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. |
| [setLogFile(String filePath)](#setLogFile-java.lang.String-) | Définit le chemin du fichier de journal et active la sortie vers le fichier (mode fichier unique, sans rotation). |
| [setLogFile(String filePath, boolean append)](#setLogFile-java.lang.String-boolean-) | Définit le chemin du fichier de journal et active la sortie vers le fichier (mode fichier unique, sans rotation). |
| [setMaxFileSize(long value)](#setMaxFileSize-long-) | Définit la taille maximale (en octets) d'un fichier de journal avant rotation. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
| [warn(String message)](#warn-java.lang.String-) | Enregistre un message de niveau avertissement. |
### closeLogFile() {#closeLogFile--}
```
public static void closeLogFile()
```


Ferme l'écrivain du fichier de journal et désactive la sortie fichier.

### debug(String message) {#debug-java.lang.String-}
```
public static void debug(String message)
```


Enregistre un message de niveau debug.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

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
### error(String message) {#error-java.lang.String-}
```
public static void error(String message)
```


Enregistre un message de niveau erreur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableConsoleOutput() {#getEnableConsoleOutput--}
```
public static boolean getEnableConsoleOutput()
```


Obtient si les messages de journal doivent être affichés dans la console. La valeur par défaut est false.

**Returns:**
boolean
### getEnableFileOutput() {#getEnableFileOutput--}
```
public static boolean getEnableFileOutput()
```


Obtient si les messages de journal doivent être écrits dans un fichier. La valeur par défaut est false. Vous devez appeler [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) ou [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) avant d'activer.

**Returns:**
boolean
### getLevel() {#getLevel--}
```
public static int getLevel()
```


Obtient le niveau de journal minimal. Les messages en dessous de ce niveau seront ignorés. La valeur par défaut est None.

Voir [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Returns:**
int
### getLogFilePath() {#getLogFilePath--}
```
public static String getLogFilePath()
```


Obtient le chemin actuel du fichier de journal, ou null s'il n'est pas défini.

**Returns:**
java.lang.String
### getMaxFileSize() {#getMaxFileSize--}
```
public static long getMaxFileSize()
```


Obtient la taille maximale (en octets) d'un fichier de journal avant rotation. Effectif uniquement lorsque la rotation est activée. 0 signifie aucune limite de taille. La valeur par défaut est 0.

**Returns:**
long
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### info(String message) {#info-java.lang.String-}
```
public static void info(String message)
```


Enregistre un message de niveau info.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

### log(int level, String message) {#log-int-java.lang.String-}
```
public static void log(int level, String message)
```


Enregistre un message au niveau spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| level | int | [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel). Le niveau de journal. |
| message | java.lang.String | Le message à enregistrer. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setEnableConsoleOutput(boolean value) {#setEnableConsoleOutput-boolean-}
```
public static void setEnableConsoleOutput(boolean value)
```


Définit si les messages de journal doivent être affichés dans la console. La valeur par défaut est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEnableFileOutput(boolean value) {#setEnableFileOutput-boolean-}
```
public static void setEnableFileOutput(boolean value)
```


Définit si les messages de journal doivent être écrits dans un fichier. La valeur par défaut est false. Vous devez appeler [setLogFile(String)](../../com.aspose.gridjs/gridjslogger\#setLogFile-String-) ou [setLogDirectory(String)](../../com.aspose.gridjs/gridjslogger\#setLogDirectory-String-) avant d'activer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLevel(int value) {#setLevel-int-}
```
public static void setLevel(int value)
```


Définit le niveau de journal minimal. Les messages en dessous de ce niveau seront ignorés. La valeur par défaut est None.

Voir [GridJsLogLevel](../../com.aspose.gridjs/gridjsloglevel).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLogDirectory(String directory) {#setLogDirectory-java.lang.String-}
```
public static void setLogDirectory(String directory)
```


Définit le répertoire de journal avec une stratégie de rotation quotidienne des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs\_\{period\}.log

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.lang.String | Le répertoire où stocker les fichiers de journal. |

### setLogDirectory(String directory, int rolling) {#setLogDirectory-java.lang.String-int-}
```
public static void setLogDirectory(String directory, int rolling)
```


Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : gridjs\_\{period\}.log

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.lang.String | Le répertoire où stocker les fichiers de journal. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La stratégie de rotation (quotidienne/hebdomadaire/mensuelle). |

### setLogDirectory(String directory, int rolling, String filePrefix) {#setLogDirectory-java.lang.String-int-java.lang.String-}
```
public static void setLogDirectory(String directory, int rolling, String filePrefix)
```


Définit le répertoire de journal avec une stratégie de rotation des fichiers et active la sortie vers le fichier. Les fichiers de journal seront nommés ainsi : \{prefix\}\_\{period\}.log Exemples : gridjs\_2026-07-27.log (quotidien), gridjs\_2026-W30.log (hebdomadaire), gridjs\_2026-07.log (mensuel)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.lang.String | Le répertoire où stocker les fichiers de journal. |
| rolling | int | [GridJsLogRolling](../../com.aspose.gridjs/gridjslogrolling). La stratégie de rotation (quotidienne/hebdomadaire/mensuelle). |
| filePrefix | java.lang.String | Le préfixe du nom de fichier. |

### setLogFile(String filePath) {#setLogFile-java.lang.String-}
```
public static void setLogFile(String filePath)
```


Définit le chemin du fichier journal et active la sortie vers le fichier (mode fichier unique, pas de rotation). Ajoute au fichier existant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin complet du fichier journal. |

### setLogFile(String filePath, boolean append) {#setLogFile-java.lang.String-boolean-}
```
public static void setLogFile(String filePath, boolean append)
```


Définit le chemin du fichier de journal et active la sortie vers le fichier (mode fichier unique, sans rotation).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le chemin complet du fichier journal. |
| ajouter | boolean | Indique s'il faut ajouter au fichier existant. |

### setMaxFileSize(long value) {#setMaxFileSize-long-}
```
public static void setMaxFileSize(long value)
```


Définit la taille maximale (en octets) d'un fichier journal unique avant rotation. Effectif uniquement lorsque la rotation est activée. 0 signifie aucune limite de taille. La valeur par défaut est 0.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | long |  |

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

### warn(String message) {#warn-java.lang.String-}
```
public static void warn(String message)
```


Enregistre un message de niveau avertissement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |

