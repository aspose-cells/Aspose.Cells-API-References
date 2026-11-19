---
title: "DateTime"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente un instant dans le temps généralement exprimé sous forme de date et d'heure."
type: docs
url: /fr/java/com.aspose.gridweb/datetime/
---

**Inheritance:**
java.lang.Object
```
public class DateTime
```

Représente un instant dans le temps, généralement exprimé sous forme de date et d'heure.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DateTime(int year, int month, int day)](#DateTime-int-int-int-) | Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois et le jour spécifiés. |
| [DateTime(int year, int month, int day, int hour, int minute, int second)](#DateTime-int-int-int-int-int-int-) | Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois, le jour, l'heure, la minute et la seconde spécifiés. |
| [DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)](#DateTime-int-int-int-int-int-int-int-) | Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois, le jour, l'heure, la minute, la seconde et la milliseconde spécifiés. |
| [DateTime(Date date)](#DateTime-java.util.Date-) | Initialise une nouvelle instance de l'objet DateTime avec l'objet Date spécifié. |
| [DateTime(Calendar cld)](#DateTime-java.util.Calendar-) | Initialise une nouvelle instance de l'objet DateTime avec l'objet Calendar spécifié. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [addDays(double value)](#addDays-double-) | Ajoute le nombre de jours spécifié à la valeur de cette instance. |
| [addHours(double value)](#addHours-double-) | Ajoute le nombre d'heures spécifié à la valeur de cette instance. |
| [addMilliseconds(double value)](#addMilliseconds-double-) | Ajoute le nombre de millisecondes spécifié à la valeur de cette instance. |
| [addMinutes(double value)](#addMinutes-double-) | Ajoute le nombre de minutes spécifié à la valeur de cette instance. |
| [addMonths(int months)](#addMonths-int-) | Ajoute le nombre de mois spécifié à la valeur de cette instance. |
| [addSeconds(double value)](#addSeconds-double-) | Ajoute le nombre de secondes spécifié à la valeur de cette instance. |
| [addYears(int value)](#addYears-int-) | Ajoute le nombre d'années spécifié à la valeur de cette instance. |
| [compareTo(DateTime value)](#compareTo-com.aspose.gridweb.DateTime-) | Compare la valeur de cette instance à une valeur DateTime spécifiée et renvoie un entier indiquant si cette instance est antérieure, identique ou postérieure à la valeur DateTime spécifiée. |
| [compareTo(Object value)](#compareTo-java.lang.Object-) | Compare la valeur de cette instance à un objet spécifié contenant une valeur DateTime, et renvoie un entier indiquant si cette instance est antérieure, identique ou postérieure à la valeur DateTime spécifiée. |
| [equals(Object value)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getClass()](#getClass--) |  |
| [getDay()](#getDay--) | Obtient le jour du mois représenté par cette instance. |
| [getDayOfWeek()](#getDayOfWeek--) | Obtient le jour de la semaine représenté par cette instance. |
| [getDayOfYear()](#getDayOfYear--) | Obtient le jour de l'année représenté par cette instance. |
| [getHour()](#getHour--) | Obtient la composante heure de la date représentée par cette instance. |
| [getMillisecond()](#getMillisecond--) | Obtient la composante millisecondes de la date représentée par cette instance. |
| [getMinute()](#getMinute--) | Obtient la composante minute de la date représentée par cette instance. |
| [getMonth()](#getMonth--) | Obtient la composante mois de la date représentée par cette instance. |
| [getNow()](#getNow--) | Obtient un objet DateTime réglé sur la date et l'heure actuelles de cet ordinateur, exprimées en heure locale. |
| [getSecond()](#getSecond--) | Obtient la composante secondes de la date représentée par cette instance. |
| [getYear()](#getYear--) | Obtient la composante année de la date représentée par cette instance. |
| [hashCode()](#hashCode--) | Renvoie le code de hachage de cette instance. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toCalendar()](#toCalendar--) | Convertit la valeur de l'objet DateTime actuel en objet Calendar. |
| [toDate()](#toDate--) | Convertit la valeur de l'objet DateTime actuel en objet Date. |
| [toLocalTime()](#toLocalTime--) | Convertit la valeur de l'objet DateTime actuel en heure locale. |
| [toString()](#toString--) | Convertit la valeur de l'objet DateTime actuel en sa représentation sous forme de chaîne équivalente. |
| [toUniversalTime()](#toUniversalTime--) | Convertit la valeur de l'objet DateTime actuel en Temps Universel Coordonné (UTC). |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DateTime(int year, int month, int day) {#DateTime-int-int-int-}
```
public DateTime(int year, int month, int day)
```


Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois et le jour spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| année | int | L'année (de 1 à 9999). |
| mois | int | Le mois (de 1 à 12). |
| jour | int | Le jour (de 1 au nombre de jours dans le mois). |

### DateTime(int year, int month, int day, int hour, int minute, int second) {#DateTime-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second)
```


Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois, le jour, l'heure, la minute et la seconde spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| année | int | L'année (de 1 à 9999). |
| mois | int | Le mois (de 1 à 12). |
| jour | int | Le jour (de 1 au nombre de jours dans le mois). |
| heure | int | Les heures (de 0 à 23). |
| minute | int | Les minutes (de 0 à 59). |
| seconde | int | Les secondes (de 0 à 59). |

### DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond) {#DateTime-int-int-int-int-int-int-int-}
```
public DateTime(int year, int month, int day, int hour, int minute, int second, int millisecond)
```


Initialise une nouvelle instance de l'objet DateTime avec l'année, le mois, le jour, l'heure, la minute, la seconde et la milliseconde spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| année | int | L'année (de 1 à 9999). |
| mois | int | Le mois (de 1 à 12). |
| jour | int | Le jour (de 1 au nombre de jours dans le mois). |
| heure | int | Les heures (de 0 à 23). |
| minute | int | Les minutes (de 0 à 59). |
| seconde | int | Les secondes (de 0 à 59). |
| milliseconde | int | Les millisecondes (de 0 à 999). |

### DateTime(Date date) {#DateTime-java.util.Date-}
```
public DateTime(Date date)
```


Initialise une nouvelle instance de l'objet DateTime avec l'objet Date spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| date | java.util.Date | L'objet Date |

### DateTime(Calendar cld) {#DateTime-java.util.Calendar-}
```
public DateTime(Calendar cld)
```


Initialise une nouvelle instance de l'objet DateTime avec l'objet Calendar spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cld | java.util.Calendar | L'objet Calendar |

### addDays(double value) {#addDays-double-}
```
public DateTime addDays(double value)
```


Ajoute le nombre de jours spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Un nombre de jours entiers et fractionnaires. Le paramètre value peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of days represented by value.
### addHours(double value) {#addHours-double-}
```
public DateTime addHours(double value)
```


Ajoute le nombre d'heures spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Un nombre d'heures entières et fractionnaires. Le paramètre value peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of hours represented by value.
### addMilliseconds(double value) {#addMilliseconds-double-}
```
public DateTime addMilliseconds(double value)
```


Ajoute le nombre de millisecondes spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Un nombre de millisecondes entières et fractionnaires. Le paramètre value peut être négatif ou positif. Notez que cette valeur est arrondie à l'entier le plus proche. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of milliseconds represented by value.
### addMinutes(double value) {#addMinutes-double-}
```
public DateTime addMinutes(double value)
```


Ajoute le nombre de minutes spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Un nombre de minutes entières et fractionnaires. Le paramètre value peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of minutes represented by value.
### addMonths(int months) {#addMonths-int-}
```
public DateTime addMonths(int months)
```


Ajoute le nombre de mois spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| mois | int | Un nombre de mois. Le paramètre months peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and months.
### addSeconds(double value) {#addSeconds-double-}
```
public DateTime addSeconds(double value)
```


Ajoute le nombre de secondes spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | Un nombre de secondes entières et fractionnaires. Le paramètre value peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of seconds represented by value.
### addYears(int value) {#addYears-int-}
```
public DateTime addYears(int value)
```


Ajoute le nombre d'années spécifié à la valeur de cette instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | Un nombre d'années. Le paramètre value peut être négatif ou positif. |

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the sum of the date and time represented by this instance and the number of years represented by value.
### compareTo(DateTime value) {#compareTo-com.aspose.gridweb.DateTime-}
```
public int compareTo(DateTime value)
```


Compare la valeur de cette instance à une valeur DateTime spécifiée et renvoie un entier indiquant si cette instance est antérieure, identique ou postérieure à la valeur DateTime spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.gridweb/datetime) | Un objet DateTime à comparer. |

**Returns:**
int - Un nombre signé indiquant les valeurs relatives de cette instance et du paramètre value. Description de la valeur Inférieure à zéro : cette instance est antérieure à value. Zéro : cette instance est identique à value. Supérieure à zéro : cette instance est postérieure à value.
### compareTo(Object value) {#compareTo-java.lang.Object-}
```
public int compareTo(Object value)
```


Compare la valeur de cette instance à un objet spécifié contenant une valeur DateTime, et renvoie un entier indiquant si cette instance est antérieure, identique ou postérieure à la valeur DateTime spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | Un objet DateTime encapsulé à comparer, ou null. |

**Returns:**
int - Un nombre signé indiquant les valeurs relatives de cette instance et de value. Description de la valeur Inférieure à zéro : cette instance est antérieure à value. Zéro : cette instance est identique à value. Supérieure à zéro : cette instance est postérieure à value, ou value est null.
### equals(Object value) {#equals-java.lang.Object-}
```
public boolean equals(Object value)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object | Un objet à comparer à cette instance. |

**Returns:**
boolean - true si value est une instance de DateTime et égale à la valeur de cette instance ; sinon, false.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDay() {#getDay--}
```
public int getDay()
```


Obtient le jour du mois représenté par cette instance.

**Returns:**
int - Le composant jour, exprimé comme une valeur entre 1 et 31.
### getDayOfWeek() {#getDayOfWeek--}
```
public int getDayOfWeek()
```


Obtient le jour de la semaine représenté par cette instance.

**Returns:**
int - le jour de la semaine de cette valeur DateTime.
### getDayOfYear() {#getDayOfYear--}
```
public int getDayOfYear()
```


Obtient le jour de l'année représenté par cette instance.

**Returns:**
int - Le jour de l'année, exprimé comme une valeur entre 1 et 366.
### getHour() {#getHour--}
```
public int getHour()
```


Obtient la composante heure de la date représentée par cette instance.

**Returns:**
int - Le composant heure, exprimé comme une valeur entre 0 et 23.
### getMillisecond() {#getMillisecond--}
```
public int getMillisecond()
```


Obtient la composante millisecondes de la date représentée par cette instance.

**Returns:**
int - Le composant millisecondes, exprimé comme une valeur entre 0 et 999.
### getMinute() {#getMinute--}
```
public int getMinute()
```


Obtient la composante minute de la date représentée par cette instance.

**Returns:**
int - Le composant minute, exprimé comme une valeur entre 0 et 59.
### getMonth() {#getMonth--}
```
public int getMonth()
```


Obtient la composante mois de la date représentée par cette instance.

**Returns:**
int - Le composant mois, exprimé comme une valeur entre 1 et 12.
### getNow() {#getNow--}
```
public static DateTime getNow()
```


Obtient un objet DateTime réglé sur la date et l'heure actuelles de cet ordinateur, exprimées en heure locale.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object whose value is the current local date and time.
### getSecond() {#getSecond--}
```
public int getSecond()
```


Obtient la composante secondes de la date représentée par cette instance.

**Returns:**
int - Les secondes, entre 0 et 59.
### getYear() {#getYear--}
```
public int getYear()
```


Obtient la composante année de la date représentée par cette instance.

**Returns:**
int - L'année, entre 1 et 9999.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie le code de hachage de cette instance.

**Returns:**
int - Un code de hachage entier signé de 32 bits.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toCalendar() {#toCalendar--}
```
public Calendar toCalendar()
```


Convertit la valeur de l'objet DateTime actuel en objet Calendar.

**Returns:**
java.util.Calendar - objet Calendar
### toDate() {#toDate--}
```
public Date toDate()
```


Convertit la valeur de l'objet DateTime actuel en objet Date.

**Returns:**
java.util.Date - objet Date
### toLocalTime() {#toLocalTime--}
```
public DateTime toLocalTime()
```


Convertit la valeur de l'objet DateTime actuel en heure locale.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of local
### toString() {#toString--}
```
public String toString()
```


Convertit la valeur de l'objet DateTime actuel en sa représentation sous forme de chaîne équivalente.

**Returns:**
java.lang.String - Une représentation sous forme de chaîne de la valeur de l'objet DateTime actuel.
### toUniversalTime() {#toUniversalTime--}
```
public DateTime toUniversalTime()
```


Convertit la valeur de l'objet DateTime actuel en Temps Universel Coordonné (UTC).

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime) - A DateTime object of UTC
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

