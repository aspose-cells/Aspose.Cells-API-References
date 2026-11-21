---
title: "Celda"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa una única celda de Workbook."
type: docs
url: /es/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Encapsula el objeto que representa una única celda de Workbook.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Métodos

| Método | Descripción |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Calcula la fórmula de la celda. |
| [characters(int startIndex, int length)](#characters-int-int-) | Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda. |
| [containsExternalLink()](#containsExternalLink--) | Indica si esta celda contiene un enlace externo. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Copia datos de una celda origen. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Comprueba si este objeto se refiere a la misma celda que otro objeto de celda. |
| [equals(Object obj)](#equals-java.lang.Object-) | Comprueba si este objeto se refiere a la misma celda que otro. |
| [getArrayRange()](#getArrayRange--) | Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz. |
| [getBoolValue()](#getBoolValue--) | Obtiene el valor booleano contenido en la celda. |
| [getCharacters()](#getCharacters--) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el número de columna (basado en cero) de la celda. |
| [getComment()](#getComment--) | Obtiene el comentario de esta celda. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Obtiene el resultado del formato condicional. |
| [getDateTimeValue()](#getDateTimeValue--) | Obtiene el valor DateTime contenido en la celda. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Obtiene todas las celdas cuya fórmula hace referencia a esta celda directamente. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Obtiene todas las celdas cuyo resultado calculado depende de esta celda. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Obtiene el valor de cadena formateado de esta celda según el estilo de visualización de la celda. |
| [getDisplayStyle()](#getDisplayStyle--) | Obtiene el estilo de visualización de esta celda. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Obtiene el estilo de visualización de esta celda. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Obtiene el estilo de visualización de esta celda. |
| [getDoubleValue()](#getDoubleValue--) | Obtiene el valor double contenido en la celda. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Obtiene la imagen incrustada en la celda. |
| [getFloatValue()](#getFloatValue--) | Obtiene el valor float contenido en la celda. |
| [getFormatConditions()](#getFormatConditions--) | Obtiene las condiciones de formato que se aplican a esta celda. |
| [getFormula()](#getFormula--) | Obtiene una fórmula de la [Cell](../../com.aspose.cells/cell). |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Obtén la fórmula de esta celda. |
| [getFormulaLocal()](#getFormulaLocal--) | Obtenga la fórmula formateada según la configuración regional de la celda. |
| [getHeightOfValue()](#getHeightOfValue--) | Obtiene la altura del valor en unidades de píxeles. |
| [getHtmlString()](#getHtmlString--) | Obtiene la cadena html que contiene datos y algunos formatos en esta celda. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Obtiene la cadena html que contiene datos y algunos formatos en esta celda. |
| [getIntValue()](#getIntValue--) | Obtiene el valor entero contenido en la celda. |
| [getLeafs()](#getLeafs--) | Obtenga todas las celdas que hacen referencia a esta celda directamente y que deben actualizarse cuando esta celda se modifica. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Obtenga todas las celdas que se actualizarán cuando esta celda se modifique. |
| [getMergedRange()](#getMergedRange--) | Devuelve un objeto [Range](../../com.aspose.cells/range) que representa un rango combinado. |
| [getName()](#getName--) | Obtiene el nombre de la celda. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Representa el tipo de categoría del formato numérico de esta celda. |
| [getPicture()](#getPicture--) | Obtiene una instancia [Picture](../../com.aspose.cells/picture) para representar la imagen incrustada en esta celda o null si no hay ninguna imagen incrustada para esta celda. |
| [getPrecedents()](#getPrecedents--) | Obtiene todas las referencias que aparecen en la fórmula de esta celda. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Obtiene todos los precedentes (referencia a celdas en el libro actual) utilizados por la fórmula de esta celda al calcularla. |
| [getR1C1Formula()](#getR1C1Formula--) | Obtiene una fórmula R1C1 de la [Cell](../../com.aspose.cells/cell). |
| [getRichValue()](#getRichValue--) | Obtiene el valor enriquecido de la celda. |
| [getRow()](#getRow--) | Obtiene el número de fila (basado en cero) de la celda. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Obtiene el índice de estilo compartido de la celda en el pool de estilos. |
| [getStringValue()](#getStringValue--) | Obtiene el valor de cadena contenido en la celda. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Obtiene el valor de cadena mediante una estrategia de formato específica. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Obtiene el valor de la celda como cadena sin ningún formato. |
| [getStyle()](#getStyle--) | Obtiene el estilo de la celda. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | Si checkBorders es true, verifica si los bordes de otras celdas afectarán el estilo de esta celda. |
| [getTable()](#getTable--) | Obtiene la tabla que contiene esta celda. |
| [getType()](#getType--) | Representa el tipo de valor de la celda. |
| [getValidation()](#getValidation--) | Obtiene la validación aplicada a esta celda. |
| [getValidationValue()](#getValidationValue--) | Obtiene el valor de la validación que se aplica a esta celda. |
| [getValue()](#getValue--) | Obtiene el valor contenido en esta celda. |
| [getWidthOfValue()](#getWidthOfValue--) | Obtiene el ancho del valor en unidades de píxeles. |
| [getWorksheet()](#getWorksheet--) | Obtiene la hoja de cálculo principal. |
| [hasCustomFunction()](#hasCustomFunction--) | Comprueba si hay una función personalizada (función no compatible) en la fórmula de esta celda. |
| [hasCustomStyle()](#hasCustomStyle--) | Indica si esta celda tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada de la fila, columna o libro de trabajo correspondiente). |
| [hashCode()](#hashCode--) | Sirve como una función hash para un tipo particular. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Inserta algunos caracteres en la celda. |
| [isArrayFormula()](#isArrayFormula--) | Indica si la fórmula de la celda es una fórmula de matriz. |
| [isArrayHeader()](#isArrayHeader--) | Indica que la fórmula de la celda es una fórmula de matriz y que es la primera celda de la matriz. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Indica si se configura esta celda como una casilla de verificación. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Indica si la fórmula de la celda es una fórmula de matriz dinámica (true) o una fórmula de matriz heredada (false). |
| [isErrorValue()](#isErrorValue--) | Comprueba si el valor de esta celda es un error. |
| [isFormula()](#isFormula--) | Representa si la celda especificada contiene una fórmula. |
| [isInArray()](#isInArray--) | Indica si la fórmula de la celda es una fórmula de matriz. |
| [isInTable()](#isInTable--) | Indica si esta celda es parte de una fórmula de tabla. |
| [isMerged()](#isMerged--) | Comprueba si una celda forma parte de un rango combinado o no. |
| [isNumericValue()](#isNumericValue--) | Indica si el valor de esta celda es numérico (int, double y datetime) |
| [isRichText()](#isRichText--) | Indica si el valor de cadena de esta celda es un texto con formato enriquecido. |
| [isSharedFormula()](#isSharedFormula--) | Indica si la fórmula de la celda es parte de una fórmula compartida. |
| [isStyleSet()](#isStyleSet--) | Indica si el estilo de la celda está configurado. |
| [isTableFormula()](#isTableFormula--) | Indica si esta celda es parte de una fórmula de tabla. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Inserta un valor booleano en la celda. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Inserta un valor DateTime en la celda. |
| [putValue(double doubleValue)](#putValue-double-) | Inserta un valor double en la celda. |
| [putValue(int intValue)](#putValue-int-) | Inserta un valor entero en la celda. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Inserta un valor de objeto en la celda. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Inserta un valor de cadena en la celda. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Inserta un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserta un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Eliminar la fórmula de matriz. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Reemplazar el texto de la celda con opciones. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Establece una fórmula de matriz (fórmula de matriz heredada introducida mediante CTRL+SHIFT+ENTER en MS Excel) en un rango de celdas. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Establece una fórmula de matriz en un rango de celdas. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Establece una fórmula de matriz en un rango de celdas. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Establece una fórmula de matriz en un rango de celdas. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Establece el formato de texto enriquecido de la celda. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Indica si se configura esta celda como una casilla de verificación. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Establece la imagen incrustada en la celda. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Establece una fórmula del [Cell](../../com.aspose.cells/cell). |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Establece la fórmula y el valor de la fórmula. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Establece la fórmula y el valor (resultado calculado) de la fórmula. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Obtenga la fórmula formateada según la configuración regional de la celda. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Establece la cadena HTML que contiene datos y algunos formatos en esta celda. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | Establece una fórmula R1C1 del [Cell](../../com.aspose.cells/cell). |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Establece fórmulas compartidas en un rango de celdas. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Establece una fórmula en un rango de celdas. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Establece fórmulas compartidas en un rango de celdas. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Establece fórmulas compartidas en un rango de celdas. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Establece el estilo de la celda. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Aplica la propiedad modificada del estilo a la celda. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Aplica el estilo de la celda según las banderas. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Crea una tabla de datos de una variable para el rango dado comenzando desde esta celda. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Crea una tabla de datos de dos variables para el rango dado comenzando desde esta celda. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Crea una tabla de datos de una variable para el rango dado comenzando desde esta celda. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Crea una tabla de datos de dos variables para el rango dado comenzando desde esta celda. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Establece el valor contenido en esta celda. |
| [toJson()](#toJson--) | Convierte el [Cell](../../com.aspose.cells/cell) a datos estructurados JSON. |
| [toString()](#toString--) | Devuelve una cadena que representa el objeto Cell actual. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Calcula la fórmula de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Opciones de cálculo |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Devuelve un objeto Characters que representa un rango de caracteres dentro del texto de la celda.

**Remarks**

Este método solo funciona en celdas con valor de cadena.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | int | El índice del inicio del carácter. |
| length | int | El número de caracteres. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indica si esta celda contiene un enlace externo. Solo se aplica cuando la celda es una celda de fórmula.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Copia datos de una celda origen.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objeto [Cell](../../com.aspose.cells/cell) de origen. |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Comprueba si este objeto se refiere a la misma celda que otro objeto de celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | otro objeto de celda |

**Returns:**
booleano - verdadero si dos objetos de celda hacen referencia a la misma celda.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Comprueba si este objeto se refiere a la misma celda que otro.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | otro objeto |

**Returns:**
booleano - verdadero si dos objetos hacen referencia a la misma celda.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Obtiene el rango de matriz si la fórmula de la celda es una fórmula de matriz.

**Remarks**

Solo se aplica cuando la fórmula de la celda es una fórmula de matriz

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Obtiene el valor booleano contenido en la celda.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda.

**Returns:**
com.aspose.cells.FontSetting[] - Todos los objetos Characters
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bandera | boolean | Indica si se aplica el estilo de tabla a la celda cuando la celda está en la tabla. |

**Returns:**
com.aspose.cells.FontSetting[] - Todos los objetos Characters
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtiene el número de columna (basado en cero) de la celda.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Obtiene el comentario de esta celda.

**Remarks**

Si no hay ningún comentario que se aplique a la celda, devuelve null.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Obtiene el resultado del formato condicional.

**Remarks**

Devuelve null si no se aplica formato condicional a esta celda,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Obtiene el valor DateTime contenido en la celda.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Obtiene todas las celdas cuya fórmula hace referencia a esta celda directamente.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isAll | boolean | Indica si se deben comprobar fórmulas en otras hojas de cálculo |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Obtiene todas las celdas cuyo resultado calculado depende de esta celda.

**Remarks**

Para usar este método, asegúrese de que el libro de trabajo se haya configurado con el valor true para [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) y se haya calculado completamente con esta configuración. Si no hay ninguna referencia de fórmula a esta celda, se devolverá null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recursive | boolean | Indica si devuelve los dependientes que no hacen referencia directamente a esta celda, sino a otras hojas derivadas de esta celda. |

**Returns:**
java.util.Iterator - Enumerador para enumerar todos los dependientes (objetos Cell)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Obtiene el valor de cadena formateado de esta celda según el estilo de visualización de la celda.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Obtiene el estilo de visualización de esta celda.

**Remarks**

Igual que usar [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) para [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-). Es decir, este método comprobará y ajustará los bordes superior/inferior/izquierdo/derecho de esta celda según el estilo ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) de sus celdas adyacentes, pero no comprobará las celdas combinadas, y no comprobará el estilo de visualización de las celdas adyacentes.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Obtiene el estilo de visualización de esta celda.

**Remarks**

Si la bandera especificada es false, entonces es lo mismo que [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--). De lo contrario, es lo mismo que usar [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) para [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| includeMergedBorders | boolean | Indica si se deben comprobar los bordes de las celdas combinadas. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Obtiene el estilo de visualización de esta celda.

**Remarks**

Si esta celda también está afectada por otras configuraciones como formato condicional, objetos de lista, etc., entonces el estilo de visualización puede ser diferente de [getStyle()](../../com.aspose.cells/cell\#getStyle--).

Para las banderas de ajuste de bordes según las celdas adyacentes, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) indican si se deben comprobar y combinar los bordes inferior/superior/derecho/izquierdo de las celdas izquierda/derecha/superior/inferior adyacentes a esta.

Por razones de rendimiento y compatibilidad, se utilizan algunos enumerados para denotar operaciones especiales:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Tenga en cuenta que comprobar los bordes/estilos de las celdas adyacentes, especialmente los estilos de visualización, es un proceso que consume tiempo. Si no es necesario obtener los bordes para el estilo devuelto, usar [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) para desactivar el proceso de celdas adyacentes proporcionará mejor rendimiento. Al obtener los bordes de las celdas adyacentes a partir de los estilos definidos solo en esas celdas (sin establecer [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)), el rendimiento también puede ser mejor porque comprobar el estilo de visualización de una celda también consume tiempo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Indica qué bordes deben ser comprobados y ajustados según los bordes de las celdas adyacentes. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Obtiene el valor double contenido en la celda.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Obtiene la imagen incrustada en la celda.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Obtiene el valor float contenido en la celda.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Obtiene las condiciones de formato que se aplican a esta celda.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - Devuelve el objeto [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Obtiene una fórmula de la [Cell](../../com.aspose.cells/cell).

**Remarks**

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor, use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Obtén la fórmula de esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | boolean | Indica si la fórmula necesita formatearse como R1C1. |
| isLocal | boolean | Indica si la fórmula necesita formatearse según la configuración regional. |

**Returns:**
java.lang.String - la fórmula de esta celda.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Obtenga la fórmula formateada según la configuración regional de la celda.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Obtiene la altura del valor en unidades de píxeles.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Obtiene la cadena html que contiene datos y algunos formatos en esta celda.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Obtiene la cadena html que contiene datos y algunos formatos en esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| html5 | boolean | Indica si el valor es compatible con html5 |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Obtiene el valor entero contenido en la celda.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Obtenga todas las celdas que hacen referencia a esta celda directamente y que deben actualizarse cuando esta celda se modifica.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo. Esta propiedad será eliminada 12 meses después, a partir de mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.util.Iterator - Enumerador para enumerar todos los dependientes(Cell)
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Obtenga todas las celdas que se actualizarán cuando esta celda se modifique.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo. Esta propiedad será eliminada 12 meses después, a partir de mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recursive | boolean | Devuelve aquellos nodos hoja que no hacen referencia a esta celda directamente, sino que hacen referencia a otras hojas de esta celda |

**Returns:**
java.util.Iterator - Enumerador para enumerar todos los dependientes(Cell)
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Devuelve un objeto [Range](../../com.aspose.cells/range) que representa un rango combinado.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre de la celda.

**Remarks**

El nombre de una celda incluye su letra de columna y número de fila. Por ejemplo, el nombre de una celda en la fila 0 y columna 0 es A1.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Representa el tipo de categoría del formato numérico de esta celda.

Ver [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Cuando el patrón de formato de la celda se combina con patrones de formato condicional, el tipo devuelto corresponde a la parte que se usa para el valor actual de esta celda. Por ejemplo, si el patrón de formato para esta celda es "\#,\#\#0;(\#,\#\#0);"-";@", entonces cuando el valor de la celda es numérico y distinto de 0, el tipo devuelto es [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER); Cuando el valor de la celda es 0 o no es un valor numérico, el tipo devuelto es [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT).

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Obtiene una instancia [Picture](../../com.aspose.cells/picture) para representar la imagen incrustada en esta celda o null si no hay ninguna imagen incrustada para esta celda.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Obtiene todas las referencias que aparecen en la fórmula de esta celda.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Obtiene todos los precedentes (referencia a celdas en el libro actual) utilizados por la fórmula de esta celda al calcularla.

**Remarks**

Este método solo puede funcionar cuando [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) es verdadero para el libro de trabajo y el libro de trabajo ha sido calculado completamente. Si esta celda no es una fórmula o no hace referencia a ninguna otra celda, se devolverá null.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - Enumerador para enumerar todas las referencias(ReferredArea)
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


Obtiene una fórmula R1C1 de la [Cell](../../com.aspose.cells/cell).

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Obtiene el valor enriquecido de la celda.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el número de fila (basado en cero) de la celda.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Obtiene el índice de estilo compartido de la celda en el pool de estilos.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es cadena, entonces devuelve el propio valor de cadena. Para otros tipos de celda, se devolverá el valor de cadena formateado (formateado con el estilo especificado de esta celda). El valor de celda formateado es el mismo que el que puede obtener de Excel al copiar una celda como texto (como copiar la celda a un editor de texto o exportar a CSV).

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Obtiene el valor de cadena mediante una estrategia de formato específica.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). La estrategia formateada. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Obtiene el valor de la celda como cadena sin ningún formato.

**Remarks**

NOTA: Este método está ahora obsoleto. En su lugar, el usuario debe obtener el objeto de valor y formatearlo según el tipo de valor y el requisito específico. Esta propiedad será eliminada 12 meses después, a partir de diciembre de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Obtiene el estilo de la celda.

**Remarks**

Para cambiar el estilo de la celda, por favor llame al método Cell.SetStyle() después de modificar el objeto de estilo devuelto. Este método es igual que [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) con el valor true para el parámetro.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


Si checkBorders es true, verifica si los bordes de otras celdas afectarán el estilo de esta celda.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| checkBorders | boolean | Comprobar los bordes de otras celdas |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Obtiene la tabla que contiene esta celda.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de valor de la celda.

Ver [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Obtiene la validación aplicada a esta celda.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Obtiene el valor de la validación que se aplica a esta celda.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Obtiene el valor contenido en esta celda.

**Remarks**

Tipo posible:

null,

Boolean,

DateTime,

Double,

Integer

String.

Para un valor int, puede devolverse como un objeto Integer o como un objeto Double. Y no hay garantía de que el valor devuelto se mantenga siempre como el mismo tipo de objeto.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Obtiene el ancho del valor en unidades de píxeles.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene la hoja de cálculo principal.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Comprueba si hay una función personalizada (función no compatible) en la fórmula de esta celda.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Indica si esta celda tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada de la fila, columna o libro de trabajo correspondiente).

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Sirve como una función hash para un tipo particular.

**Returns:**
int - Un código hash para el objeto Cell actual.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Inserte algunos caracteres en la celda. Si la celda tiene formato enriquecido, este método podría conservar el formato original.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | El índice. |
| texto | java.lang.String | Texto insertado. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Indica si la fórmula de la celda es una fórmula de matriz.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Indica que la fórmula de la celda es una fórmula de matriz y que es la primera celda de la matriz.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Indica si se configura esta celda como una casilla de verificación.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Indica si la fórmula de la celda es una fórmula de matriz dinámica (true) o una fórmula de matriz heredada (false).

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Comprueba si el valor de esta celda es un error.

**Remarks**

También se aplica a la celda de fórmula para comprobar si el resultado calculado es un error.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Representa si la celda especificada contiene una fórmula.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Indica si la fórmula de la celda es una fórmula de matriz.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.IsArrayFormula para comprobar si la fórmula de la celda es una fórmula de matriz. Esta propiedad será eliminada 12 meses después desde mayo de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Indica si esta celda es parte de una fórmula de tabla.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.IsTableFormula para comprobar si la fórmula de la celda forma parte de una fórmula de tabla. Esta propiedad será eliminada 12 meses después desde mayo de 2018. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Comprueba si una celda forma parte de un rango combinado o no.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Indica si el valor de esta celda es numérico (int, double y datetime)

**Remarks**

También se aplica a la celda de fórmula para comprobar el resultado calculado

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Indica si el valor de cadena de esta celda es un texto con formato enriquecido.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Indica si la fórmula de la celda es parte de una fórmula compartida.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indica si el estilo de la celda está establecido. Si devuelve false, significa que esta celda tiene un formato de celda predeterminado.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Indica si esta celda es parte de una fórmula de tabla.

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




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Inserta un valor booleano en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Inserta un valor DateTime en la celda.

**Remarks**

Establecer un valor DateTime para una celda no significa que la celda se formatee automáticamente como fecha y hora. El valor DateTime se mantiene como un valor numérico en el modelo de datos tanto de MS Excel como de Aspose.Cells. Si el valor numérico se interpretará como el propio valor numérico o como fecha y hora depende del formato numérico aplicado a esta celda. Si esta celda no ha sido formateada como fecha y hora, se mostrará como un valor numérico aunque lo que ingresó sea DateTime.

**Example**

Este ejemplo muestra cómo establecer un valor DateTime en una celda y hacer que se muestre como fecha y hora.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Valor de entrada |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Inserta un valor double en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| doubleValue | double | Valor de entrada |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Inserta un valor entero en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| intValue | int | Valor de entrada |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Inserta un valor de objeto en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| objectValue | java.lang.Object | valor de entrada |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Inserta un valor de cadena en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Inserta un valor de cadena en la celda y convierte el valor a otro tipo de datos si es apropiado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Inserta un valor en la celda; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de la celda se restablecerá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | java.lang.String | Valor de entrada |
| isConverted | boolean | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | boolean | True: establece el formato numérico en el estilo de la celda al convertir a otro tipo de datos |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Eliminar la fórmula de matriz.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| leaveNormalFormula | boolean | True representa la conversión de la fórmula de matriz a fórmula normal. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Reemplazar el texto de la celda con opciones.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | java.lang.String | Marcador de posición de celda |
| newValue | java.lang.String | Valor de cadena para reemplazar |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Las opciones de reemplazo |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Establece una fórmula de matriz (fórmula de matriz heredada introducida mediante CTRL+SHIFT+ENTER en MS Excel) en un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | Fórmula de matriz. |
| rowNumber | int | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | int | Número de columnas para poblar el resultado de la fórmula de matriz. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Establece una fórmula de matriz en un rango de celdas.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Esta propiedad será eliminada 12 meses después desde diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | Fórmula de matriz. |
| rowNumber | int | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | int | Número de columnas para poblar el resultado de la fórmula de matriz. |
| isR1C1 | boolean | si la fórmula es una fórmula R1C1 |
| isLocal | boolean | si la fórmula está formateada según la configuración regional |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Establece una fórmula de matriz en un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | Fórmula de matriz. |
| rowNumber | int | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | int | Número de columnas para poblar el resultado de la fórmula de matriz. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Establece una fórmula de matriz en un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | Fórmula de matriz. |
| rowNumber | int | Número de filas para poblar el resultado de la fórmula de matriz. |
| columnNumber | int | Número de columnas para poblar el resultado de la fórmula de matriz. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |
| valores | java.lang.Object[][] | valores para esas celdas con la fórmula de matriz dada |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Establece el formato de texto enriquecido de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Todos los objetos Characters. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Indica si se configura esta celda como una casilla de verificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

**Remarks**

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se desborda. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "\#SPILL!". Pero para este tipo de situación todavía devolvemos todo el rango en el que esta fórmula debería desbordarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | la expresión de la fórmula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| calculateValue | boolean | si calcular esta fórmula de matriz dinámica para esas celdas en el rango desbordado. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

**Remarks**

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se desborda. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "\#SPILL!". Pero para este tipo de situación todavía devolvemos todo el rango en el que esta fórmula debería desbordarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | la expresión de la fórmula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| valores | java.lang.Object[][] | valores (resultados calculados) para esas celdas con la fórmula de matriz dinámica dada |
| calculateRange | boolean | si calcular el rango desbordado para esta fórmula de matriz dinámica. Si el parámetro "values" no es nulo y esta bandera es falsa, entonces la altura del rango desbordado será values.Length y el ancho será values[0].Length. |
| calculateValue | boolean | si calcular esta fórmula de matriz dinámica para esas celdas en el rango desbordado cuando "values" es nulo o el elemento correspondiente en "values" para una celda es nulo. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Establece una fórmula de matriz dinámica y hace que la fórmula se desborde a celdas vecinas si es posible.

**Remarks**

el rango devuelto puede no ser el mismo que el real en el que esta fórmula de matriz dinámica se desborda. Si hay celdas no vacías en el rango, la fórmula se establecerá solo para la celda actual y se marcará como "\#SPILL!". Pero para este tipo de situación todavía devolvemos todo el rango en el que esta fórmula debería desbordarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arrayFormula | java.lang.String | la expresión de la fórmula |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | opciones para analizar la fórmula. La opción "Parse" será ignorada y la fórmula siempre se analizará inmediatamente |
| valores | java.lang.Object[][] | valores (resultados calculados) para esas celdas con la fórmula de matriz dinámica dada |
| calculateRange | boolean | si calcular el rango desbordado para esta fórmula de matriz dinámica. Si el parámetro "values" no es nulo y esta bandera es falsa, entonces la altura del rango desbordado será values.Length y el ancho será values[0].Length. |
| calculateValue | boolean | si calcular esta fórmula de matriz dinámica para esas celdas en el rango desbordado cuando "values" es nulo o el elemento correspondiente en "values" para una celda es nulo. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Las opciones para calcular la fórmula. Normalmente, por consideraciones de rendimiento, la propiedad [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\#getRecursive--) debería ser false. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Establece la imagen incrustada en la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Establece una fórmula del [Cell](../../com.aspose.cells/cell).

**Remarks**

Una cadena de fórmula siempre comienza con un signo igual (=). Y por favor, use siempre la coma (,) como delimitador de parámetros, como "=SUM(A1, E1, H2)".

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Establece la fórmula y el valor de la fórmula.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, por favor use Cell.SetFormula(string,FormulaParseOptions,object). Esta propiedad será eliminada 12 meses después desde diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula. |
| isR1C1 | boolean | Si la fórmula es una fórmula R1C1. |
| isLocal | boolean | Si la fórmula está formateada según la configuración regional. |
| valor | java.lang.Object | El valor de la fórmula. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Establece la fórmula y el valor (resultado calculado) de la fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Establece la fórmula y el valor (resultado calculado) de la fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |
| valor | java.lang.Object | El valor (resultado calculado) de la fórmula. |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Establece la fórmula y el valor (resultado calculado) de la fórmula.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formula | java.lang.String | La fórmula. |
| valor | java.lang.Object | El valor (resultado calculado) de la fórmula. |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Obtenga la fórmula formateada según la configuración regional de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Establece la cadena HTML que contiene datos y algunos formatos en esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


Establece una fórmula R1C1 del [Cell](../../com.aspose.cells/cell).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Establece fórmulas compartidas en un rango de celdas.

**Remarks**

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | java.lang.String | Fórmula compartida. |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Establece una fórmula en un rango de celdas.

**Remarks**

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Esta propiedad será eliminada 12 meses después desde diciembre de 2019. Aspose se disculpa por cualquier inconveniente que haya experimentado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | java.lang.String | Fórmula compartida. |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| isR1C1 | boolean | si la fórmula es una fórmula R1C1 |
| isLocal | boolean | si la fórmula está formateada según la configuración regional |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Establece fórmulas compartidas en un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | java.lang.String | Fórmula compartida. |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Establece fórmulas compartidas en un rango de celdas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sharedFormula | java.lang.String | Fórmula compartida. |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Opciones para analizar la fórmula. |
| valores | java.lang.Object[][] | valores para esas celdas con la fórmula compartida dada |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Establece el estilo de la celda.

**Remarks**

Si se cambian los ajustes del borde, el borde de las celdas ajustadas también se actualizará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El estilo de la celda. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Aplica la propiedad modificada del estilo a la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El estilo de la celda. |
| explicitFlag | boolean | Verdadero, solo sobrescribiendo el formato que está establecido explícitamente. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Aplica el estilo de la celda según las banderas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | El estilo de la celda. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | El indicador de estilo. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Crea una tabla de datos de una variable para el rango dado comenzando desde esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| rowIndexOfInputCell | int | índice de fila de la celda de entrada |
| columnIndexOfInputCell | int | índice de columna de la celda de entrada |
| isRowInput | boolean | Indica si la celda de entrada es una celda de entrada de fila (true) o una celda de entrada de columna (false). |
| valores | java.lang.Object[][] | valores para celdas en el rango de fórmula de la tabla |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Crea una tabla de datos de dos variables para el rango dado comenzando desde esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| rowIndexOfRowInputCell | int | índice de fila de la celda de entrada de fila |
| columnIndexOfRowInputCell | int | índice de columna de la celda de entrada de fila |
| rowIndexOfColumnInputCell | int | índice de fila de la celda de entrada de columna |
| columnIndexOfColumnInputCell | int | índice de columna de la celda de entrada de columna |
| valores | java.lang.Object[][] | valores para celdas en el rango de fórmula de la tabla |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Crea una tabla de datos de una variable para el rango dado comenzando desde esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| inputCell | java.lang.String | la celda de entrada |
| isRowInput | boolean | Indica si la celda de entrada es una celda de entrada de fila (true) o una celda de entrada de columna (false). |
| valores | java.lang.Object[][] | valores para celdas en el rango de fórmula de la tabla |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Crea una tabla de datos de dos variables para el rango dado comenzando desde esta celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowNumber | int | Número de filas para poblar la fórmula. |
| columnNumber | int | Número de columnas para poblar la fórmula. |
| rowInputCell | java.lang.String | la celda de entrada de fila |
| columnInputCell | java.lang.String | la celda de entrada de columna |
| valores | java.lang.Object[][] | valores para celdas en el rango de fórmula de la tabla |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Establece el valor contenido en esta celda.

**Remarks**

Tipo posible:

null,

Boolean,

DateTime,

Double,

Integer

String.

Para un valor int, puede devolverse como un objeto Integer o como un objeto Double. Y no hay garantía de que el valor devuelto se mantenga siempre como el mismo tipo de objeto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


Convierte el [Cell](../../com.aspose.cells/cell) a datos estructurados JSON.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Devuelve una cadena que representa el objeto Cell actual.

**Returns:**
java.lang.String -
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

