---
title: "TextBoxActiveXControl"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет элемент управления ActiveX текстовым полем."
type: docs
url: /ru/java/com.aspose.cells/textboxactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class TextBoxActiveXControl extends ActiveXControl
```

Представляет элемент управления ActiveX текстовым полем.

**Example**

```
         //Initialize a new workbook.
         Workbook book = new Workbook();
 
         //Add a TextBoxActiveXControl.
         Shape shape = book.getWorksheets().get(0).getShapes().addActiveXControl(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50);
         TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.getActiveXControl();
 
         //do your business
 
         //Save the excel file.
         book.save("exmaple.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Получает OLE‑цвет фона. |
| [getBorderOleColor()](#getBorderOleColor--) | Получает OLE‑цвет фона. |
| [getBorderStyle()](#getBorderStyle--) | Получает тип границы, используемой элементом управления. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Получает двоичные данные элемента управления. |
| [getDropButtonStyle()](#getDropButtonStyle--) | Указывает символ, отображаемый на кнопке раскрытия |
| [getEnterFieldBehavior()](#getEnterFieldBehavior--) | Указывает поведение выбора при входе в элемент управления. |
| [getEnterKeyBehavior()](#getEnterKeyBehavior--) | Указывает поведение клавиши ENTER. |
| [getFont()](#getFont--) | Представляет шрифт элемента управления. |
| [getForeOleColor()](#getForeOleColor--) | Получает OLE‑цвет переднего плана. |
| [getHeight()](#getHeight--) | Получает высоту элемента управления в пунктах. |
| [getHideSelection()](#getHideSelection--) | Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса. |
| [getIMEMode()](#getIMEMode--) | Получает режим выполнения по умолчанию редактора методов ввода для элемента управления при получении им фокуса. |
| [getIntegralHeight()](#getIntegralHeight--) | Указывает, будет ли элемент управления показывать только полные строки текста, не показывая частичные строки. |
| [getLinkedCell()](#getLinkedCell--) | Получает связанную ячейку. |
| [getListFillRange()](#getListFillRange--) | Получает диапазон заполнения списка. |
| [getMaxLength()](#getMaxLength--) | Получает максимальное количество символов |
| [getMouseIcon()](#getMouseIcon--) | Получает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [getMousePointer()](#getMousePointer--) | Получает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [getPasswordChar()](#getPasswordChar--) | Получает символ, который будет отображаться вместо введённых символов. |
| [getScrollBars()](#getScrollBars--) | Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни один. |
| [getShadow()](#getShadow--) | Указывает, отображать ли тень. |
| [getShowDropButtonTypeWhen()](#getShowDropButtonTypeWhen--) | Указывает символ, отображаемый на кнопке раскрытия |
| [getSpecialEffect()](#getSpecialEffect--) | Получает специальный эффект элемента управления. |
| [getTabKeyBehavior()](#getTabKeyBehavior--) | Указывает, разрешены ли символы табуляции в тексте элемента управления. |
| [getText()](#getText--) | Получает текст элемента управления. |
| [getTextAlign()](#getTextAlign--) | Представляет способ выравнивания текста, используемого элементом управления. |
| [getType()](#getType--) | Получает тип ActiveX‑элемента управления. |
| [getWidth()](#getWidth--) | Получает ширину элемента управления в единицах точек. |
| [getWorkbook()](#getWorkbook--) | Получает объект [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--). |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [isAutoTab()](#isAutoTab--) | Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов. |
| [isAutoWordSelected()](#isAutoWordSelected--) | Задает базовую единицу, используемую для расширения выделения. |
| [isDragBehaviorEnabled()](#isDragBehaviorEnabled--) | Указывает, включено ли перетаскивание для элемента управления. |
| [isEditable()](#isEditable--) | Указывает, может ли пользователь вводить данные в элемент управления. |
| [isEnabled()](#isEnabled--) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [isLocked()](#isLocked--) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [isMultiLine()](#isMultiLine--) | Указывает, может ли элемент управления отображать более одной строки текста. |
| [isTransparent()](#isTransparent--) | Указывает, является ли элемент управления прозрачным. |
| [isVisible()](#isVisible--) | Указывает, видим ли этот элемент управления. |
| [isWordWrapped()](#isWordWrapped--) | Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Указывает, будет ли элемент управления автоматически изменять размер для отображения всего содержимого. |
| [setAutoTab(boolean value)](#setAutoTab-boolean-) | Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов. |
| [setAutoWordSelected(boolean value)](#setAutoWordSelected-boolean-) | Задает базовую единицу, используемую для расширения выделения. |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | Устанавливает OLE‑цвет фона. |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Устанавливает тип границы, используемой элементом управления. |
| [setDragBehaviorEnabled(boolean value)](#setDragBehaviorEnabled-boolean-) | Указывает, включено ли перетаскивание для элемента управления. |
| [setDropButtonStyle(int value)](#setDropButtonStyle-int-) | Указывает символ, отображаемый на кнопке раскрытия |
| [setEditable(boolean value)](#setEditable-boolean-) | Указывает, может ли пользователь вводить данные в элемент управления. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Указывает, может ли элемент управления получать фокус и реагировать на события, генерируемые пользователем. |
| [setEnterFieldBehavior(boolean value)](#setEnterFieldBehavior-boolean-) | Указывает поведение выбора при входе в элемент управления. |
| [setEnterKeyBehavior(boolean value)](#setEnterKeyBehavior-boolean-) | Указывает поведение клавиши ENTER. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Устанавливает OLE‑цвет переднего плана. |
| [setHeight(double value)](#setHeight-double-) | Устанавливает высоту элемента управления в единицах точек. |
| [setHideSelection(boolean value)](#setHideSelection-boolean-) | Указывает, выделяется ли выбранный текст в элементе управления, когда элемент не имеет фокуса. |
| [setIMEMode(int value)](#setIMEMode-int-) | Устанавливает режим выполнения по умолчанию для Input Method Editor элемента управления при получении фокуса. |
| [setIntegralHeight(boolean value)](#setIntegralHeight-boolean-) | Указывает, будет ли элемент управления показывать только полные строки текста, не показывая частичные строки. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает связанную ячейку. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Устанавливает диапазон заполнения списка. |
| [setLocked(boolean value)](#setLocked-boolean-) | Указывает, заблокированы ли данные в элементе управления для редактирования. |
| [setMaxLength(int value)](#setMaxLength-int-) | Устанавливает максимальное количество символов |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Устанавливает пользовательский значок, отображаемый в качестве указателя мыши для элемента управления. |
| [setMousePointer(int value)](#setMousePointer-int-) | Устанавливает тип значка, отображаемого в качестве указателя мыши для элемента управления. |
| [setMultiLine(boolean value)](#setMultiLine-boolean-) | Указывает, может ли элемент управления отображать более одной строки текста. |
| [setPasswordChar(char value)](#setPasswordChar-char-) | Устанавливает символ, который будет отображаться вместо введённых символов. |
| [setScrollBars(int value)](#setScrollBars-int-) | Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни один. |
| [setShadow(boolean value)](#setShadow-boolean-) | Указывает, отображать ли тень. |
| [setShowDropButtonTypeWhen(int value)](#setShowDropButtonTypeWhen-int-) | Указывает символ, отображаемый на кнопке раскрытия |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | Устанавливает специальный эффект элемента управления. |
| [setTabKeyBehavior(boolean value)](#setTabKeyBehavior-boolean-) | Указывает, разрешены ли символы табуляции в тексте элемента управления. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текст элемента управления. |
| [setTextAlign(int value)](#setTextAlign-int-) | Представляет способ выравнивания текста, используемого элементом управления. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Указывает, является ли элемент управления прозрачным. |
| [setVisible(boolean value)](#setVisible-boolean-) | Указывает, видим ли этот элемент управления. |
| [setWidth(double value)](#setWidth-double-) | Устанавливает ширину элемента управления в единицах пунктов. |
| [setWordWrapped(boolean value)](#setWordWrapped-boolean-) | Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки. |
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

**Example**

```
         //excel default color system 12 or green(0x0000FF00)
         activeXControl.setBorderOleColor(/*unchecked*/((int)0x80000012L));
```

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Получает тип границы, используемой элементом управления.

См. [ControlBorderType](../../com.aspose.cells/controlbordertype).

**Example**

```
         activeXControl.setBorderStyle(com.aspose.cells.ControlBorderType.SINGLE);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

**Example**

```
         activeXControl.setDropButtonStyle(com.aspose.cells.DropButtonStyle.ARROW);
```

**Returns:**
int
### getEnterFieldBehavior() {#getEnterFieldBehavior--}
```
public boolean getEnterFieldBehavior()
```


Указывает поведение выбора при входе в элемент управления. True указывает, что выбор остаётся неизменным с последнего раза, когда элемент управления был активен. False указывает, что весь текст в элементе управления будет выбран при входе в элемент управления.

**Example**

```
         if(!activeXControl.getEnterFieldBehavior())
         {
             activeXControl.setEnterFieldBehavior(true);
         }
```

**Returns:**
boolean
### getEnterKeyBehavior() {#getEnterKeyBehavior--}
```
public boolean getEnterKeyBehavior()
```


Указывает поведение клавиши ENTER. True указывает, что нажатие ENTER создаст новую строку. False указывает, что нажатие ENTER переместит фокус к следующему объекту в порядке табуляции.

**Example**

```
         if(!activeXControl.getEnterKeyBehavior())
         {
             activeXControl.setEnterKeyBehavior(true);
         }
```

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

**Example**

```
         if(!activeXControl.getHideSelection())
         {
             activeXControl.setHideSelection(true);
         }
```

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
### getIntegralHeight() {#getIntegralHeight--}
```
public boolean getIntegralHeight()
```


Указывает, будет ли элемент управления показывать только полные строки текста, не показывая частичные строки.

**Example**

```
         if(!activeXControl.getIntegralHeight())
         {
             activeXControl.setIntegralHeight(true);
         }
```

**Returns:**
boolean
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
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Получает максимальное количество символов

**Example**

```
         if(activeXControl.getMaxLength() == 0)
         {
             activeXControl.setMaxLength(30);
         }
```

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
### getPasswordChar() {#getPasswordChar--}
```
public char getPasswordChar()
```


Получает символ, который будет отображаться вместо введённых символов.

**Example**

```
         activeXControl.setPasswordChar('a');
```

**Returns:**
char
### getScrollBars() {#getScrollBars--}
```
public int getScrollBars()
```


Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни один.

Смотрите [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Example**

```
         activeXControl.setScrollBars(com.aspose.cells.ControlScrollBarType.BARS_VERTICAL);
```

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Указывает, отображать ли тень.

**Returns:**
boolean
### getShowDropButtonTypeWhen() {#getShowDropButtonTypeWhen--}
```
public int getShowDropButtonTypeWhen()
```


Указывает символ, отображаемый на кнопке раскрытия

См. [ShowDropButtonType](../../com.aspose.cells/showdropbuttontype).

**Example**

```
         activeXControl.setShowDropButtonTypeWhen(com.aspose.cells.ShowDropButtonType.FOCUS);
```

**Returns:**
int
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


Получает специальный эффект элемента управления.

См. [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype).

**Example**

```
         activeXControl.setSpecialEffect(com.aspose.cells.ControlSpecialEffectType.BUMP);
```

**Returns:**
int
### getTabKeyBehavior() {#getTabKeyBehavior--}
```
public boolean getTabKeyBehavior()
```


Указывает, разрешены ли символы табуляции в тексте элемента управления.

**Example**

```
         if(!activeXControl.getTabKeyBehavior())
         {
             activeXControl.setTabKeyBehavior(true);
         }
```

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Получает текст элемента управления.

**Example**

```
         activeXControl.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


Представляет способ выравнивания текста, используемого элементом управления.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Получает тип ActiveX‑элемента управления.

См. [ControlType](../../com.aspose.cells/controltype).

**Example**

```
         /*Aspose.Cells.Drawing.ActiveXControls.ControlType*/int type = activeXControl.getType();
```

**Returns:**
int
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
### isAutoTab() {#isAutoTab--}
```
public boolean isAutoTab()
```


Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов.

**Example**

```
         if(!activeXControl.isAutoTab())
         {
             activeXControl.setAutoTab(true);
         }
```

**Returns:**
boolean
### isAutoWordSelected() {#isAutoWordSelected--}
```
public boolean isAutoWordSelected()
```


Указывает базовую единицу, используемую для расширения выделения. True указывает, что базовая единица — один символ. false указывает, что базовая единица — целое слово.

**Example**

```
         if(!activeXControl.isAutoWordSelected())
         {
             activeXControl.setAutoWordSelected(true);
         }
```

**Returns:**
boolean
### isDragBehaviorEnabled() {#isDragBehaviorEnabled--}
```
public boolean isDragBehaviorEnabled()
```


Указывает, включено ли перетаскивание для элемента управления.

**Example**

```
         if(!activeXControl.isDragBehaviorEnabled())
         {
             activeXControl.setDragBehaviorEnabled(true);
         }
```

**Returns:**
boolean
### isEditable() {#isEditable--}
```
public boolean isEditable()
```


Указывает, может ли пользователь вводить данные в элемент управления.

**Example**

```
         if(!activeXControl.isEditable())
         {
             activeXControl.setEditable(true);
         }
```

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
### isMultiLine() {#isMultiLine--}
```
public boolean isMultiLine()
```


Указывает, может ли элемент управления отображать более одной строки текста.

**Example**

```
         if(!activeXControl.isMultiLine())
         {
             activeXControl.setMultiLine(true);
         }
```

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
### isWordWrapped() {#isWordWrapped--}
```
public boolean isWordWrapped()
```


Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки.

**Example**

```
         if(!activeXControl.isWordWrapped())
         {
             activeXControl.setWordWrapped(true);
         }
```

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

### setAutoTab(boolean value) {#setAutoTab-boolean-}
```
public void setAutoTab(boolean value)
```


Указывает, будет ли фокус автоматически перемещаться к следующему элементу управления, когда пользователь вводит максимальное количество символов.

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

### setEnterKeyBehavior(boolean value) {#setEnterKeyBehavior-boolean-}
```
public void setEnterKeyBehavior(boolean value)
```


Указывает поведение клавиши ENTER. True указывает, что нажатие ENTER создаст новую строку. False указывает, что нажатие ENTER переместит фокус к следующему объекту в порядке табуляции.

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

### setIntegralHeight(boolean value) {#setIntegralHeight-boolean-}
```
public void setIntegralHeight(boolean value)
```


Указывает, будет ли элемент управления показывать только полные строки текста, не показывая частичные строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Указывает, заблокированы ли данные в элементе управления для редактирования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setMultiLine(boolean value) {#setMultiLine-boolean-}
```
public void setMultiLine(boolean value)
```


Указывает, может ли элемент управления отображать более одной строки текста.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPasswordChar(char value) {#setPasswordChar-char-}
```
public void setPasswordChar(char value)
```


Устанавливает символ, который будет отображаться вместо введённых символов.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | char |  |

### setScrollBars(int value) {#setScrollBars-int-}
```
public void setScrollBars(int value)
```


Указывает, имеет ли элемент управления вертикальные полосы прокрутки, горизонтальные полосы прокрутки, оба типа или ни один.

Смотрите [ControlScrollBarType](../../com.aspose.cells/controlscrollbartype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Указывает, отображать ли тень.

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

### setTabKeyBehavior(boolean value) {#setTabKeyBehavior-boolean-}
```
public void setTabKeyBehavior(boolean value)
```


Указывает, разрешены ли символы табуляции в тексте элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает текст элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

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

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Указывает, является ли элемент управления прозрачным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setWordWrapped(boolean value) {#setWordWrapped-boolean-}
```
public void setWordWrapped(boolean value)
```


Указывает, будет ли содержимое элемента управления автоматически переноситься в конце строки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

