---
title: "AbstractCalculationEngine"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells."
type: docs
url: /fr/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

**Remarks**

L'utilisateur ne doit pas modifier directement aucune partie du classeur dans cette implémentation (excepté le résultat calculé de la fonction personnalisée, qui peut être défini via la propriété CalculationData.CalculatedValue). Sinon, un résultat inattendu ou une exception peut survenir. Si l'utilisateur doit modifier d'autres données que le résultat calculé dans l'implémentation pour certaines fonctions personnalisées, par exemple modifier la formule d'une cellule, le style, etc., il doit rassembler ces données dans cette implémentation et les modifier en dehors du périmètre du calcul de formule.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Calcule une fonction avec les données fournies. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Indique s'il faut forcer la fonction donnée à être recalculée systématiquement lors du calcul des formules partagées. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Indique si les fonctions intégrées prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indique si ce moteur nécessite que le paramètre soit calculé en mode tableau. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indique si ce moteur a besoin du texte littéral du paramètre lors d'un calcul. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Ignore le calcul de toute la formule qui référence la fonction actuellement évaluée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


Calcule une fonction avec les données fournies.

**Remarks**

L'utilisateur doit définir la valeur calculée pour les données données pour toutes les fonctions (y compris les fonctions natives d'Excel) qu'il souhaite calculer lui‑même dans cette implémentation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | les données requises pour calculer la fonction telles que le nom de la fonction, les paramètres, ...etc. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Indique s'il faut forcer la fonction donnée à être recalculée systématiquement lors du calcul des formules partagées.

**Remarks**

Pour les formules partagées, plusieurs cellules partagent la même fonction. Si les paramètres de la fonction restent identiques pour ces cellules, cette fonction doit généralement être calculée une seule fois. Ainsi, pour des raisons de performance, nous ne calculons ce type de fonction qu'une fois également ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) n'est appelé qu'une fois, au lieu d'être appelé à plusieurs reprises pour chaque cellule). Cependant, dans l'implémentation personnalisée de l'utilisateur, il se peut que la fonction, en particulier la fonction personnalisée, doive être calculée différemment selon les cellules. Dans ce cas, l'utilisateur doit remplacer cette méthode pour qu'elle renvoie true pour la fonction. Et pour [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), le [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) fourni peut avoir été initialisé avec la valeur mise en cache du calcul précédent.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionName | java.lang.String | nom de la fonction. En général, il s'agit du nom de la fonction personnalisée. Si [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) est vrai, les fonctions intégrées seront également vérifiées ici. |

**Returns:**
booléen - true si la fonction spécifiée doit être recalculée systématiquement.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Indique si les fonctions intégrées prises en charge par le moteur intégré doivent être vérifiées et traitées par cette implémentation. La valeur par défaut est false.

**Remarks**

Si l'utilisateur doit modifier la logique de calcul de certaines fonctions intégrées, cette propriété doit être définie sur true. Sinon, veuillez laisser cette propriété sur false pour des raisons de performance.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


Indique si ce moteur nécessite que le paramètre soit calculé en mode tableau. La valeur par défaut est false. Si [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) est requis lors du calcul de fonctions personnalisées et que l'utilisateur n'a pas mis à jour la définition correspondante (via [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), cette propriété doit être définie sur true.

**Remarks**

Si ce moteur de calcul personnalisé nécessite que le paramètre soit calculé en mode tableau, davantage de piles seront requises pour mettre en cache l'arbre des paramètres et la méthode Calculate() pourra être appelée de manière récursive pour calculer la valeur du paramètre. Pour des raisons de performance, veuillez conserver cette propriété à sa valeur par défaut (false) s'il n'y a aucune exigence particulière.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Indique si ce moteur a besoin du texte littéral du paramètre lors d'un calcul. La valeur par défaut est false.

**Remarks**

Si ce moteur de calcul personnalisé a besoin du texte littéral du paramètre, davantage de piles seront nécessaires pour mettre en cache le texte littéral des paramètres et la méthode Calculate() pourra être appelée de manière récursive pour calculer la valeur du paramètre. En général, le texte littéral n'est pas nécessaire pour le calcul des formules et cette propriété doit rester à false pour la plupart des implémentations afin d'obtenir de meilleures performances.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Ignore le calcul de toute la formule qui référence la fonction actuellement évaluée.

**Remarks**

Cette méthode peut être invoquée dans l'implémentation de [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) pour ignorer le calcul de toute la formule et la valeur originale de la formule sera conservée sans modification.

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

