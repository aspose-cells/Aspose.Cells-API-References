---
title: "PivotGlobalizationSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres de mondialisation pour les tableaux croisés dynamiques."
type: docs
url: /fr/java/com.aspose.cells/pivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotGlobalizationSettings
```

Représente les paramètres de mondialisation pour les tableaux croisés dynamiques.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PivotGlobalizationSettings()](#PivotGlobalizationSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | Obtient le format numérique du groupe de jour du tableau croisé dynamique. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | Obtient le nom d'affichage du champ de données du tableau croisé dynamique. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | Obtient toutes les chaînes courtes formatées des 12 mois. |
| [getTextOf24Hours()](#getTextOf24Hours--) | Obtient toutes les chaînes formatées localement des 24 heures. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | Obtient le texte local des 4 trimestres. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | Obtient le texte local des 4 trimestres. |
| [getTextOfAll()](#getTextOfAll--) | Obtient le texte de l'étiquette \"(All)\" dans le tableau croisé dynamique. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | Obtient le texte localisé de \"All Periods\". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | Obtient le texte de l'étiquette \"Column Labels\" dans le tableau croisé dynamique. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | Obtient le texte de l'en-tête du champ de zone de valeur dans le PivotTable. |
| [getTextOfDays()](#getTextOfDays--) | Obtient le texte local de "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | Obtient le texte de l'étiquette "(blank)" dans le PivotTable. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | Obtient le texte de l'étiquette "Grand Total" dans le PivotTable. |
| [getTextOfHours()](#getTextOfHours--) | Obtient le texte local de "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | Obtient le texte local de "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | Obtient le texte local de "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | Obtient le texte de l'étiquette "(Multiple Items)" dans le PivotTable. |
| [getTextOfOr()](#getTextOfOr--) | Obtient toutes les chaînes formatées localement de "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | Obtient le texte pour le nom protégé spécifié. |
| [getTextOfProtection()](#getTextOfProtection--) | Obtient le nom de protection dans le tableau croisé dynamique. |
| [getTextOfQuarters()](#getTextOfQuarters--) | Obtient le texte local de "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | Obtient le texte local de "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | Obtient le texte de l'étiquette "Row Labels" dans le PivotTable. |
| [getTextOfSeconds()](#getTextOfSeconds--) | Obtient le texte local de "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | Obtient le texte du type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) dans le PivotTable. |
| [getTextOfTotal()](#getTextOfTotal--) | Obtient le texte de l'étiquette "Total" dans le PivotTable. |
| [getTextOfYears()](#getTextOfYears--) | Obtient le texte local de "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotGlobalizationSettings() {#PivotGlobalizationSettings--}
```
public PivotGlobalizationSettings()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


Obtient le format numérique du groupe de jour du tableau croisé dynamique. Utilisé uniquement lors du regroupement du champ de tableau croisé dynamique par jour. La valeur par défaut est "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


Obtient le nom d'affichage du champ de données du tableau croisé dynamique. Le format par défaut est "Sum Of Field".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). La fonction est utilisée pour résumer les valeurs du champ de tableau croisé dynamique. |
| name | java.lang.String | Le nom original du champ de tableau croisé dynamique. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


Obtient toutes les chaînes courtes formatées des 12 mois.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


Obtient toutes les chaînes formatées localement des 24 heures. La valeur par défaut est 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


Obtient le texte local des 4 trimestres.

**Remarks**

Renvoie par défaut Quarter1, Quarter2, Quarter3, Quarter4 avant la version 26.9. Renvoie par défaut Qtr1, Qtr2, Qtr3, Qtr4 depuis la version 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


Obtient le texte local des 4 trimestres.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetTextOf4Quarters(). Cette propriété sera supprimée 12 mois plus tard à compter de juillet 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


Obtient le texte de l'étiquette \"(All)\" dans le tableau croisé dynamique.

**Returns:**
java.lang.String - Le texte de l'étiquette "(All)"
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


Obtient le texte localisé de \"All Periods\".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


Obtient le texte de l'étiquette \"Column Labels\" dans le tableau croisé dynamique.

**Returns:**
java.lang.String - Le texte des étiquettes de colonne
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


Obtient le texte de l'en-tête du champ de zone de valeur dans le PivotTable.

**Returns:**
java.lang.String - Le texte du nom d’en-tête du champ de données
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


Obtient le texte local de "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


Obtient le texte de l'étiquette "(blank)" dans le PivotTable.

**Returns:**
java.lang.String - Le texte des données vides
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


Obtient le texte de l'étiquette "Grand Total" dans le PivotTable.

**Returns:**
java.lang.String - Le texte de l’étiquette "Grand Total"
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


Obtient le texte local de "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


Obtient le texte local de "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


Obtient le texte local de "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


Obtient le texte de l'étiquette "(Multiple Items)" dans le PivotTable.

**Returns:**
java.lang.String - Le texte de l’étiquette "(Multiple Items)"
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


Obtient toutes les chaînes formatées localement de "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


Obtient le texte pour le nom protégé spécifié.

**Remarks**

Dans Ms Excel, certains noms ne sont pas autorisés à être utilisés comme nom de PivotFields dans un PivotTable. Ils varient selon les régions ; l'utilisateur peut les spécifier explicitement en fonction de la région utilisée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| protectedName | java.lang.String | Le nom protégé dans le PivotTable. |

**Returns:**
java.lang.String - Les noms protégés locaux du PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


Obtient le nom de protection dans le tableau croisé dynamique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode PivotGlobalizationSettings.GetTextOfProtectedName(string). Cette propriété sera supprimée 12 mois plus tard à compter de mars 2023. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
java.lang.String - Le nom de protection du tableau croisé dynamique
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


Obtient le texte local de "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


Obtient le texte local de "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


Obtient le texte de l'étiquette "Row Labels" dans le PivotTable.

**Returns:**
java.lang.String - Le texte des étiquettes de ligne
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


Obtient le texte local de "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


Obtient le texte du type [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) dans le PivotTable.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). Le [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - Le texte du type donné
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


Obtient le texte de l’étiquette "Total" dans le PivotTable. Vous devez remplacer cette méthode lorsque le PivotTable contient deux champs ou plus dans la zone de données.

**Returns:**
java.lang.String - Le texte de l’étiquette "Total"
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


Obtient le texte local de "Years".

**Returns:**
java.lang.String -
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

