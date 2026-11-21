---
title: "Validering"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar data validation.settings."
type: docs
url: /sv/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

Representerar data validation.settings.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Tillämpar valideringen på området. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Tillämpar valideringen på området. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Tillämpar valideringen på angivna områden. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Kopiera validering. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Representerar stilen för valideringsvarningen. |
| [getAreas()](#getAreas--) | Hämtar alla [CellArea](../../com.aspose.cells/cellarea) som innehåller inställningarna för datavalidering. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Representerar felmeddelandet för datavalidering. |
| [getErrorTitle()](#getErrorTitle--) | Representerar titeln på felmeddelanderutan för datavalidering. |
| [getFormula1()](#getFormula1--) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Hämtar värdet eller uttrycket som är kopplat till denna validering. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Hämtar värdet eller uttrycket som är associerat med den här valideringen för en specifik cell. |
| [getFormula2()](#getFormula2--) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Hämtar värdet eller uttrycket som är kopplat till denna validering. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Hämtar värdet eller uttrycket som är associerat med den här valideringen för en specifik cell. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Anger om tomma värden är tillåtna av områdets datavalidering. |
| [getInCellDropDown()](#getInCellDropDown--) | Anger om datavalidering visar en rullgardinslista som innehåller godkända värden. |
| [getInputMessage()](#getInputMessage--) | Representerar datavalideringens inmatningsmeddelande. |
| [getInputTitle()](#getInputTitle--) | Representerar titeln på datavalideringens inmatningsdialogruta. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Hämta värdet för listan av valideringen för den angivna cellen. |
| [getOperator()](#getOperator--) | Representerar operatorn för datavalideringen. |
| [getShowError()](#getShowError--) | Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data. |
| [getShowInput()](#getShowInput--) | Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet. |
| [getType()](#getType--) | Representerar datavalideringstypen. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Hämta värdet av valideringen på den specifika cellen. |
| [getValue1()](#getValue1--) | Representerar det första värdet som är associerat med datavalideringen. |
| [getValue2()](#getValue2--) | Representerar det andra värdet som är associerat med datavalideringen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Ta bort valideringsinställningarna i cellen. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Ta bort valideringsinställningarna i området. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Tar bort den här valideringen från angivna områden. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Representerar stilen för valideringsvarningen. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Representerar felmeddelandet för datavalidering. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Representerar titeln på felmeddelanderutan för datavalidering. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Ställer in värdet eller uttrycket som är associerat med den här valideringen. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Representerar värdet eller uttrycket som är kopplat till datavalideringen. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Ställer in värdet eller uttrycket som är associerat med den här valideringen. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Anger om tomma värden är tillåtna av områdets datavalidering. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Anger om datavalidering visar en rullgardinslista som innehåller godkända värden. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Representerar datavalideringens inmatningsmeddelande. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Representerar titeln på datavalideringens inmatningsdialogruta. |
| [setOperator(int value)](#setOperator-int-) | Representerar operatorn för datavalideringen. |
| [setShowError(boolean value)](#setShowError-boolean-) | Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet. |
| [setType(int value)](#setType-int-) | Representerar datavalideringstypen. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Representerar det första värdet som är associerat med datavalideringen. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Representerar det andra värdet som är associerat med datavalideringen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


Tillämpar valideringen på området.

**Remarks**

Det är ekvivalent att använda [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) med kontroll av korsning och kant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Området. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


Tillämpar valideringen på området.

**Remarks**

I den här metoden kommer vi att ta bort alla gamla valideringar i det angivna området. För den översta vänstra av Valideringens tillämpade områden är först dess StartRow den minsta, därefter är dess StartColumn den minsta av de områden som har samma minsta StartRow.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Området. |
| checkIntersection | boolean | Om korsningen av det angivna området med befintliga valideringsområden ska kontrolleras. Om en validering har tillämpats i det angivna området (eller en del av det), bör den befintliga valideringen först tas bort från det angivna området. Annars kan korruption uppstå för de genererade valideringarna. Om användaren är säker på att det tillagda området inte korsar något befintligt område kan denna parameter sättas till false för prestandaskäl. |
| checkEdge | boolean | Om kanten av denna validerings tillämpade områden ska kontrolleras. Valideringens interna inställningar beror på den översta vänstra av dess tillämpade områden, så om det angivna området blir det nya översta vänstra området, bör de interna inställningarna ändras och byggas om, annars kan oväntade resultat uppstå. Om användaren är säker på att det tillagda området inte är det översta vänstra, kan denna parameter sättas till false för prestandaskäl. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


Tillämpar valideringen på angivna områden.

**Remarks**

I den här metoden kommer vi att ta bort alla gamla valideringar i det angivna området. För den översta vänstra av Valideringens tillämpade områden är först dess StartRow den minsta, därefter är dess StartColumn den minsta av de områden som har samma minsta StartRow.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | Områdena. |
| checkIntersection | boolean | Om kontrollera korsningen av det angivna området med befintliga valideringsområden. Om en validering har tillämpats i det angivna området (eller en del av det), bör den befintliga valideringen först tas bort från det angivna området. Annars kan korruption uppstå för de genererade valideringarna. Om användaren är säker på att alla tillagda områden inte korsar något befintligt område, kan denna parameter sättas till false av prestandaskäl. |
| checkEdge | boolean | Om kontrollera kanten av denna validerings tillämpade områden. Valideringens interna inställningar beror på det översta vänstra området av dess tillämpade intervall, så om ett av de angivna områdena blir det nya översta vänstra intervallet, bör de interna inställningarna ändras och byggas om, annars kan ett oväntat resultat uppstå. Om användaren är säker på att inget av de tillagda områdena är det översta vänstra, kan denna parameter sättas till false av prestandaskäl. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


Kopiera validering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | Källvalideringen. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | Kopieringsalternativet. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


Representerar stilen för valideringsvarningen.

Se [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Hämtar alla [CellArea](../../com.aspose.cells/cellarea) som innehåller inställningarna för datavalidering.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


Representerar felmeddelandet för datavalidering.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


Representerar titeln på felmeddelanderutan för datavalidering.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


Hämtar värdet eller uttrycket som är kopplat till denna validering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med denna validering.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


Hämtar värdet eller uttrycket som är associerat med den här valideringen för en specifik cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med denna validering.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


Hämtar värdet eller uttrycket som är kopplat till denna validering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med denna validering.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


Hämtar värdet eller uttrycket som är associerat med den här valideringen för en specifik cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | boolean | Om formeln behöver formateras som R1C1. |
| isLocal | boolean | Om formeln behöver formateras enligt lokala inställningar. |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.String - Värdet eller uttrycket som är associerat med denna validering.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


Anger om tomma värden är tillåtna av områdets datavalidering.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


Anger om datavalidering visar en rullgardinslista som innehåller godkända värden.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


Representerar datavalideringens inmatningsmeddelande.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


Representerar titeln på datavalideringens inmatningsdialogruta.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


Hämta värdet för listan av valideringen för den angivna cellen.

**Remarks**

Endast för validering vars typ är List och som har tillämpats på den angivna cellen, annars returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

**Returns:**
java.lang.Object - Värdet för att skapa listan för denna validering för den angivna cellen. Om listan refererar till ett område, kommer det returnerade värdet att vara ett [ReferredArea](../../com.aspose.cells/referredarea)-objekt; annars kan det returnerade värdet vara null, object[] eller ett enkelt objekt.
### getOperator() {#getOperator--}
```
public int getOperator()
```


Representerar operatorn för datavalideringen.

Se [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Representerar datavalideringstypen.

Se [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


Hämta värdet av valideringen på den specifika cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |
| isValue1 | boolean | Indikerar om det första värdet hämtas. |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


Representerar det första värdet som är associerat med datavalideringen.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


Representerar det andra värdet som är associerat med datavalideringen.

**Returns:**
java.lang.Object
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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


Ta bort valideringsinställningarna i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindexet. |
| kolumn | int | Kolumnindexet. |

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


Ta bort valideringsinställningarna i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | områdena där dessa valideringsinställningar ska tas bort. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


Tar bort den här valideringen från angivna områden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | områdena där dessa valideringsinställningar ska tas bort. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


Representerar stilen för valideringsvarningen.

Se [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


Representerar felmeddelandet för datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


Representerar titeln på felmeddelanderutan för datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


Ställer in värdet eller uttrycket som är associerat med den här valideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


Representerar värdet eller uttrycket som är kopplat till datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


Ställer in värdet eller uttrycket som är associerat med den här valideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Värdet eller uttrycket som är associerat med detta formatvillkor. |
| isR1C1 | boolean | Om formeln är en R1C1-formel. |
| isLocal | boolean | Om formeln är lokalanpassad. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


Anger om tomma värden är tillåtna av områdets datavalidering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


Anger om datavalidering visar en rullgardinslista som innehåller godkända värden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


Representerar datavalideringens inmatningsmeddelande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


Representerar titeln på datavalideringens inmatningsdialogruta.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


Representerar operatorn för datavalideringen.

Se [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


Anger om datavalideringens felmeddelande ska visas när användaren anger ogiltiga data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


Anger om datavalideringens inmatningsmeddelande ska visas när användaren markerar en cell i datavalideringsområdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Representerar datavalideringstypen.

Se [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


Representerar det första värdet som är associerat med datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


Representerar det andra värdet som är associerat med datavalideringen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

