---
title: "ComboBoxActiveXControl"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет элемент управления ComboBox ActiveX."
type: docs
url: /ru/java/com.aspose.cells/comboboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ComboBoxActiveXControl extends ActiveXControl
```

Представляет элемент управления ComboBox ActiveX.
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Получает OLE‑цвет фона. |
| [getBorderOleColor()](#getBorderOleColor--) | Получает OLE‑цвет фона. |
| [getBorderStyle()](#getBorderStyle--) | Получает тип границы, используемой элементом управления. |
| [getBoundColumn()](#getBoundColumn--) | Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle). |
| [getClass()](#getClass--) |  |
| [getColumnCount()](#getColumnCount--) | Представляет количество столбцов, отображаемых в ComboBox или ListBox. |
| [getColumnWidths()](#getColumnWidths--) | Получает ширину столбца. |
| [getData()](#getData--) | Получает двоичные данные элемента управления. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Указывает символ, отображаемый на кнопке раскрытия |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Указывает поведение выбора при входе в элемент управления. |
| [getFont()](#getFont--) | Представляет шрифт элемента управления. |
| [getForeOleColor()](#getForeOleColor--) | Получает OLE‑цвет переднего плана. |
| [getHeight()](#getHeight--) | Получает высоту элемента управления в пунктах. |
| [getHideSelection()](#getHideSelection--) | Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса. |
| [getIMEMode()](#getIMEMode--) | Получает режим выполнения по умолчанию редактора методов ввода для элемента управления при получении им фокуса. |
| [getLinkedCell()](#getLinkedCell--) | Получает связанную ячейку. |
| [getListFillRange()](#getListFillRange--) | Получает диапазон заполнения списка. |
| [getListRows()](#getListRows--) | Представляет максимальное количество строк, отображаемых в списке. |
| [getListStyle()](#getListStyle--) | Получает визуальное оформление. |
| [getListWidth()](#getListWidth--) | Получает ширину в пунктах. |
| [getMatchEntry()](#getMatchEntry--) | Указывает, как ListBox или ComboBox ищут в списке при вводе пользователем. |
| [getMaxLength()](#getMaxLength--) | Получает максимальное количество символов |
| [getMouseIcon()](#getMouseIcon--) | Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [getMousePointer()](#getMousePointer--) | Получает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [getSelectionMargin()](#getSelectionMargin--) | Указывает, может ли пользователь выбрать строку текста, щёлкнув в области слева от текста. |
| [getShadow()](#getShadow--) | Указывает, отображать ли тень. |
| [getShowColumnHeads()](#getShowColumnHeads--) | Указывает, отображаются ли заголовки столбцов. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Указывает символ, отображаемый на кнопке раскрытия |
| [getSpecialEffect()](#getSpecialEffect--) | Получает специальный эффект элемента управления. |
| [getTextAlign()](#getTextAlign--) | Представляет способ выравнивания текста, используемого элементом управления. |
| [getTextColumn()](#getTextColumn--) | Представляет столбец в ComboBox или ListBox, отображаемый пользователю. |
| [getType()](#getType--) | Получает тип ActiveX‑элемента управления. |
| [getValue()](#getValue--) | Получает значение элемента управления. |
| [getWidth()](#getWidth--) | Получает ширину элемента управления в единицах точек. |
| [getWorkbook()](#getWorkbook--) | Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Задает базовую единицу, используемую для расширения выделения. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Указывает, включено ли перетаскивание для элемента управления. |
| [isEditable()](#isEditable--) | Указывает, может ли пользователь вводить данные в элемент управления. |
| [isEnabled()](#isEnabled--) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [isLocked()](#isLocked--) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [isTransparent()](#isTransparent--) | Указывает, является ли элемент управления прозрачным. |
| [isVisible()](#isVisible--) | Указывает, видим ли этот элемент управления. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Задает базовую единицу, используемую для расширения выделения. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Устанавливает тип границы, используемой элементом управления. |
| [setBoundColumn(int value)](#setBoundColumn-int-) | Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle). |
| [setColumnCount(int value)](#setColumnCount-int-) | Представляет количество столбцов, отображаемых в ComboBox или ListBox. |
| [setColumnWidths(double value)](#setColumnWidths-double-) | Устанавливает ширину столбца. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Указывает, включено ли перетаскивание для элемента управления. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Указывает символ, отображаемый на кнопке раскрытия |
| [setEditable(boolean value)](#setEditable-boolean-) | Указывает, может ли пользователь вводить данные в элемент управления. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Указывает поведение выбора при входе в элемент управления. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Устанавливает OLE‑цвет переднего плана. |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту элемента управления в единицах точек. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса. |
| [setIMEMode(int value)](#setIMEMode-int-) | Устанавливает режим выполнения по умолчанию для Input Method Editor элемента управления при получении фокуса. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает связанную ячейку. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Устанавливает диапазон заполнения списка. |
| [setListRows(int value)](#setListRows-int-) | Представляет максимальное количество строк, отображаемых в списке. |
| [setListStyle(int value)](#setListStyle-int-) | Устанавливает визуальный вид. |
| [setListWidth(double value)](#setListWidth-double-) | Устанавливает ширину в единицах точек. |
| [setLocked(boolean value)](#setLocked-boolean-) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [setMatchEntry(int value)](#setMatchEntry-int-) | Указывает, как ListBox или ComboBox ищут в списке при вводе пользователем. |
| [setMaxLength(int value)](#setMaxLength-int-) | Устанавливает максимальное количество символов |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [setMousePointer(int value)](#setMousePointer-int-) | Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [setSelectionMargin(boolean value)](#setSelectionMargin-boolean-) | Указывает, может ли пользователь выбрать строку текста, щёлкнув в области слева от текста. |
| [setShadow(boolean value)](#setShadow-boolean-) | Указывает, отображать ли тень. |
| [setShowColumnHeads(boolean value)](#setShowColumnHeads-boolean-) | Указывает, отображаются ли заголовки столбцов. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Указывает символ, отображаемый на кнопке раскрытия |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Устанавливает специальный эффект элемента управления. |
| [setTextAlign(int value)](#setTextAlign-int-) | Представляет способ выравнивания текста, используемого элементом управления. |
| [setTextColumn(int value)](#setTextColumn-int-) | Представляет столбец в ComboBox или ListBox, отображаемый пользователю. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Указывает, является ли элемент управления прозрачным. |
| [setValue(String value)](#setValue-java.lang.String-) | Устанавливает значение элемента управления. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, видим ли этот элемент управления. |
| [setWidth(double value)](#setWidth-double-) | Устанавливает ширину элемента управления в единицах пунктов. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Получает OLE‑цвет фона.

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


Получает OLE‑цвет фона.

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Получает тип границы, используемой элементом управления.

См. [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Returns:**
int
### getBoundColumn() {#getBoundColumn--}
```
public int getBoundColumn()
```


Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCount() {#getColumnCount--}
```
public int getColumnCount()
```


Представляет количество столбцов, отображаемых в ComboBox или ListBox.

**Returns:**
int
### getColumnWidths() {#getColumnWidths--}
```
public double getColumnWidths()
```


Получает ширину столбца.

**Returns:**
double
### getData() {#getData--}
```
public byte[] getData()
```


Получает двоичные данные элемента управления.

**Returns:**
byte[]
### getDropButtonStyle() {#getDropButtonStyle--}
```
public int getDropButtonStyle()
```


Указывает символ, отображаемый на кнопке раскрытия

См. [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Указывает поведение выбора при входе в элемент управления. True указывает, что выбор остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выбран при входе в элемент управления.

**Returns:**
boolean
### getFont() {#getFont--}
```
public Font getFont()
```


Представляет шрифт элемента управления.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Получает OLE‑цвет переднего плана.

**Remarks**

Не применяется к элементу управления Image.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Получает высоту элемента управления в пунктах.

**Returns:**
double
### getHideSelection() {#getHideSelection--}
```
public boolean getHideSelection()
```


Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса.

**Returns:**
boolean
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


Получает режим выполнения по умолчанию редактора методов ввода для элемента управления при получении им фокуса.

См. [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Получает связанную ячейку.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Получает диапазон заполнения списка.

**Returns:**
java.lang.String
### getListRows() {#getListRows--}
```
public int getListRows()
```


Представляет максимальное количество строк, отображаемых в списке.

**Returns:**
int
### getListStyle() {#getListStyle--}
```
public int getListStyle()
```


Получает визуальное оформление.

См. [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Returns:**
int
### getListWidth() {#getListWidth--}
```
public double getListWidth()
```


Получает ширину в пунктах.

**Returns:**
double
### getMatchEntry() {#getMatchEntry--}
```
public int getMatchEntry()
```


Указывает, как ListBox или ComboBox ищут в списке при вводе пользователем.

См. [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Returns:**
int
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Получает максимальное количество символов

**Returns:**
int
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Получает тип значка, отображаемого в качестве указателя мыши для элемента управления.

См. [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getSelectionMargin() {#getSelectionMargin--}
```
public boolean getSelectionMargin()
```


Указывает, может ли пользователь выбрать строку текста, щёлкнув в области слева от текста.

**Returns:**
boolean
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Указывает, отображать ли тень.

**Returns:**
boolean
### getShowColumnHeads() {#getShowColumnHeads--}
```
public boolean getShowColumnHeads()
```


Указывает, отображаются ли заголовки столбцов.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Указывает символ, отображаемый на кнопке раскрытия

См. [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Получает специальный эффект элемента управления.

См. [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Представляет способ выравнивания текста, используемого элементом управления.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextColumn() {#getTextColumn--}
```
public int getTextColumn()
```


Представляет столбец в ComboBox или ListBox, отображаемый пользователю.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Получает тип ActiveX‑элемента управления.

См. [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getValue() {#getValue--}
```
public String getValue()
```


Получает значение элемента управления.

**Returns:**
java.lang.String
### getWidth() {#getWidth--}
```
public double getWidth()
```


Получает ширину элемента управления в единицах точек.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--).

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Указывает базовую единицу, используемую для расширения выделения. True указывает, что базовая единица — один символ. false указывает, что базовая единица — целое слово.

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Указывает, включено ли перетаскивание для элемента управления.

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Указывает, может ли пользователь вводить данные в элемент управления.

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Указывает, заблокированы ли данные в элементе управления для редактирования.

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


Указывает, является ли элемент управления прозрачным.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Указывает, видим ли этот элемент управления.

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoWordSelected(boolean value) {#setAutoWordSelected-boolean-}
```
public void setAutoWordSelected(boolean value)
```


Указывает базовую единицу, используемую для расширения выделения. True указывает, что базовая единица — один символ. false указывает, что базовая единица — целое слово.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Устанавливает OLE‑цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


Устанавливает OLE‑цвет фона.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Устанавливает тип границы, используемой элементом управления.

См. [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBoundColumn(int value) {#setBoundColumn-int-}
```
public void setBoundColumn(int value)
```


Представляет, как определяется свойство Value для ComboBox или ListBox, когда значение свойства MultiSelect равно (fmMultiSelectSingle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColumnCount(int value) {#setColumnCount-int-}
```
public void setColumnCount(int value)
```


Представляет количество столбцов, отображаемых в ComboBox или ListBox.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColumnWidths(double value) {#setColumnWidths-double-}
```
public void setColumnWidths(double value)
```


Устанавливает ширину столбца.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setDragBehaviorEnabled(boolean value) {#setDragBehaviorEnabled-boolean-}
```
public void setDragBehaviorEnabled(boolean value)
```


Указывает, включено ли перетаскивание для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setDropButtonStyle(int value) {#setDropButtonStyle-int-}
```
public void setDropButtonStyle(int value)
```


Указывает символ, отображаемый на кнопке раскрытия

См. [DropButtonStyle](../../com.aspose.cells/dropbuttonstyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setEditable(boolean value) {#setEditable-boolean-}
```
public void setEditable(boolean value)
```


Указывает, может ли пользователь вводить данные в элемент управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setEnterFieldBehavior(boolean value) {#setEnterFieldBehavior-boolean-}
```
public void setEnterFieldBehavior(boolean value)
```


Указывает поведение выбора при входе в элемент управления. True указывает, что выбор остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выбран при входе в элемент управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Устанавливает OLE‑цвет переднего плана.

**Remarks**

Не применяется к элементу управления Image.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Устанавливает высоту элемента управления в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHideSelection(boolean value) {#setHideSelection-boolean-}
```
public void setHideSelection(boolean value)
```


Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


Устанавливает режим выполнения по умолчанию для Input Method Editor элемента управления при получении фокуса.

См. [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Устанавливает связанную ячейку.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Устанавливает диапазон заполнения списка.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setListRows(int value) {#setListRows-int-}
```
public void setListRows(int value)
```


Представляет максимальное количество строк, отображаемых в списке.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setListStyle(int value) {#setListStyle-int-}
```
public void setListStyle(int value)
```


Устанавливает визуальный вид.

См. [ControlListStyle](../../com.aspose.cells/controlliststyle).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setListWidth(double value) {#setListWidth-double-}
```
public void setListWidth(double value)
```


Устанавливает ширину в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Указывает, заблокированы ли данные в элементе управления для редактирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMatchEntry(int value) {#setMatchEntry-int-}
```
public void setMatchEntry(int value)
```


Указывает, как ListBox или ComboBox ищут в списке при вводе пользователем.

См. [ControlMatchEntryType](../../com.aspose.cells/controlmatchentrytype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Устанавливает максимальное количество символов

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления.

См. [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSelectionMargin(boolean value) {#setSelectionMargin-boolean-}
```
public void setSelectionMargin(boolean value)
```


Указывает, может ли пользователь выбрать строку текста, щёлкнув в области слева от текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Указывает, отображать ли тень.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowColumnHeads(boolean value) {#setShowColumnHeads-boolean-}
```
public void setShowColumnHeads(boolean value)
```


Указывает, отображаются ли заголовки столбцов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowDropButtonTypeWhen(int value) {#setShowDropButtonTypeWhen-int-}
```
public void setShowDropButtonTypeWhen(int value)
```


Указывает символ, отображаемый на кнопке раскрытия

См. [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


Устанавливает специальный эффект элемента управления.

См. [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


Представляет способ выравнивания текста, используемого элементом управления.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextColumn(int value) {#setTextColumn-int-}
```
public void setTextColumn(int value)
```


Представляет столбец в ComboBox или ListBox, отображаемый пользователю.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Указывает, является ли элемент управления прозрачным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setValue(String value) {#setValue-java.lang.String-}
```
public void setValue(String value)
```


Устанавливает значение элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Указывает, видим ли этот элемент управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Устанавливает ширину элемента управления в единицах пунктов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

