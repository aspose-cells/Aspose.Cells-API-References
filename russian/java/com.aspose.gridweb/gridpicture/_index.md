---
title: "GridPicture"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий отдельное изображение в электронных таблицах."
type: docs
url: /ru/java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Инкапсулирует объект, представляющий отдельное изображение в электронных таблицах.
## Методы

| Метод | Описание |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Добавляет гиперссылку к фигуре. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Перемещает изображение в правый верхний угол. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Возвращает или задаёт описательную (альтернативную) строку текста объекта [GridShape](../../com.aspose.gridweb/gridshape). |
| [getBorderLineColor()](#getBorderLineColor--) | Представляет [Color](../../com.aspose.cells/color) границы линии изображения. |
| [getBorderWeight()](#getBorderWeight--) | Получает толщину границы линии изображения в единицах pt. |
| [getBottom()](#getBottom--) | Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Получает данные изображения. |
| [getHeight()](#getHeight--) | Представляет высоту фигуры в пикселях. |
| [getHeightCM()](#getHeightCM--) | Представляет высоту фигуры в дюймах. |
| [getHeightInch()](#getHeightInch--) | Представляет высоту фигуры в дюймах. |
| [getHeightPt()](#getHeightPt--) | Представляет высоту фигуры в пунктах. |
| [getHeightScale()](#getHeightScale--) | Получает масштаб высоты в процентах от исходной высоты изображения. |
| [getHtmlText()](#getHtmlText--) | Получает HTML-строку, содержащую данные и некоторые форматирования в этом текстовом поле. |
| [getHyperlink()](#getHyperlink--) | Получает гиперссылку фигуры. |
| [getID()](#getID--) | Получает/устанавливает ID изображения. |
| [getImageFormat()](#getImageFormat--) | Получает формат изображения. |
| [getLeft()](#getLeft--) | Представляет горизонтальное смещение фигуры от её левого столбца в пикселях. |
| [getLeftCM()](#getLeftCM--) | Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах. |
| [getLeftInch()](#getLeftInch--) | Представляет горизонтальное смещение фигуры от её левого столбца в дюймах. |
| [getLeftToCorner()](#getLeftToCorner--) | Представляет горизонтальное смещение фигуры от левого края листа, в пикселях. |
| [getLinkedCell()](#getLinkedCell--) | Получает диапазон листа, связанный со значением элемента управления. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Получает горизонтальное смещение фигуры от столбца её нижнего правого угла. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Получает вертикальное смещение фигуры от строки её нижнего правого угла. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Представляет индекс столбца нижнего правого угла. |
| [getLowerRightRow()](#getLowerRightRow--) | Представляет индекс строки нижнего правого угла. |
| [getName()](#getName--) | Получает имя фигуры. |
| [getOriginalHeight()](#getOriginalHeight--) | Получает исходную высоту изображения. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Получает исходную высоту изображения в сантиметрах. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Получает исходную высоту изображения в дюймах. |
| [getOriginalWidth()](#getOriginalWidth--) | Получает исходную ширину изображения. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Получает исходную ширину изображения в сантиметрах. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Получает исходную ширину изображения в дюймах. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Указывает, является ли фигура относительной к оригинальному размеру изображения. |
| [getRight()](#getRight--) | Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях. |
| [getRotationAngle()](#getRotationAngle--) | Получает вращение фигуры. |
| [getSourceFullName()](#getSourceFullName--) | Получает путь и имя исходного файла для связанного изображения. |
| [getText()](#getText--) | Представляет строку в этом объекте TextBox. |
| [getTitle()](#getTitle--) | Указывает заголовок (подпись) текущего объекта фигуры. |
| [getTop()](#getTop--) | Представляет вертикальное смещение фигуры от её верхней строки, в пикселях. |
| [getTopCM()](#getTopCM--) | Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах. |
| [getTopInch()](#getTopInch--) | Представляет вертикальное смещение фигуры от её верхней строки, в дюймах. |
| [getTopToCorner()](#getTopToCorner--) | Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Получает горизонтальное смещение фигуры от её столбца в левом верхнем углу. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Получает вертикальное смещение фигуры от её строки в левом верхнем углу. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Представляет индекс столбца левого верхнего угла. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Представляет индекс строки верхнего левого угла. |
| [getWidth()](#getWidth--) | Представляет ширину фигуры в пикселях. |
| [getWidthCM()](#getWidthCM--) | Представляет ширину фигуры в сантиметрах. |
| [getWidthInch()](#getWidthInch--) | Представляет ширину фигуры в дюймах. |
| [getWidthPt()](#getWidthPt--) | Представляет ширину фигуры в пунктах. |
| [getWidthScale()](#getWidthScale--) | Получает масштаб ширины в процентах от исходной ширины изображения. |
| [getX()](#getX--) | Получает горизонтальное смещение фигуры от левого края листа, в пикселях. |
| [getY()](#getY--) | Получает вертикальное смещение фигуры от верхнего края листа в пикселях. |
| [getZOrderPosition()](#getZOrderPosition--) | Возвращает позицию фигуры в порядке Z. |
| [hasLine()](#hasLine--) | Получает, видима ли линия границы фигуры. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Получает, отражена ли фигура по вертикали. |
| [isGroup()](#isGroup--) | Указывает, является ли фигура группой. |
| [isHidden()](#isHidden--) | Указывает, видим ли объект. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True означает, что изменения соотношения сторон не допускаются. |
| [isLocked()](#isLocked--) | True, если объект заблокирован, False, если объект может быть изменён, когда лист защищён. |
| [isTextWrapped()](#isTextWrapped--) | Получает тип переноса текста у объекта, содержащего текст. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Перемещает изображение в указанное место. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Перемещает объект в указанный диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Удалить гиперссылку фигуры. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Создаёт изображение и сохраняет его в поток. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Возвращает или задаёт описательную (альтернативную) строку текста объекта [GridShape](../../com.aspose.gridweb/gridshape). |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Представляет [Color](../../com.aspose.cells/color) границы линии изображения. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Устанавливает толщину границы изображения в пунктах. |
| [setBottom(int value)](#setBottom-int-) | Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях. |
| [setData(byte[] value)](#setData-byte---) | Получает данные изображения. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Устанавливает, будет ли объект отражён по вертикали. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Устанавливает видимость границы линии объекта. |
| [setHeight(int value)](#setHeight-int-) | Представляет высоту фигуры в пикселях. |
| [setHeightCM(double value)](#setHeightCM-double-) | Представляет высоту фигуры в дюймах. |
| [setHeightInch(double value)](#setHeightInch-double-) | Представляет высоту фигуры в дюймах. |
| [setHeightPt(double value)](#setHeightPt-double-) | Представляет высоту фигуры в пунктах. |
| [setHeightScale(int value)](#setHeightScale-int-) | Устанавливает масштаб высоты в процентах от исходной высоты изображения. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, видим ли объект. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Устанавливает HTML‑строку, содержащую данные и некоторые форматирования, в этом текстовом поле. |
| [setID(String value)](#setID-java.lang.String-) | Получает/устанавливает ID изображения. |
| [setLeft(int value)](#setLeft-int-) | Представляет горизонтальное смещение фигуры от её левого столбца в пикселях. |
| [setLeftCM(double value)](#setLeftCM-double-) | Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах. |
| [setLeftInch(double value)](#setLeftInch-double-) | Представляет горизонтальное смещение фигуры от её левого столбца в дюймах. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Представляет горизонтальное смещение фигуры от левого края листа, в пикселях. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает диапазон листа, связанный со значением элемента управления. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True означает, что изменения соотношения сторон не допускаются. |
| [setLocked(boolean value)](#setLocked-boolean-) | True, если объект заблокирован, False, если объект может быть изменён, когда лист защищён. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Устанавливает горизонтальное смещение объекта от столбца его нижнего правого угла. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Устанавливает вертикальное смещение объекта от строки его нижнего правого угла. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Представляет индекс столбца нижнего правого угла. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Представляет индекс строки нижнего правого угла. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя объекта. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Указывает, является ли фигура относительной к оригинальному размеру изображения. |
| [setRight(int value)](#setRight-int-) | Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Устанавливает вращение объекта. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Устанавливает путь и имя исходного файла для связанного изображения. |
| [setText(String value)](#setText-java.lang.String-) | Представляет строку в этом объекте TextBox. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Устанавливает тип переноса текста в фигуре, содержащей текст. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Указывает заголовок (подпись) текущего объекта фигуры. |
| [setTop(int value)](#setTop-int-) | Представляет вертикальное смещение фигуры от её верхней строки, в пикселях. |
| [setTopCM(double value)](#setTopCM-double-) | Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах. |
| [setTopInch(double value)](#setTopInch-double-) | Представляет вертикальное смещение фигуры от её верхней строки, в дюймах. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Устанавливает горизонтальное смещение фигуры от столбца её верхнего левого угла. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Устанавливает вертикальное смещение фигуры от строки её верхнего левого угла. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Представляет индекс столбца левого верхнего угла. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Представляет индекс строки верхнего левого угла. |
| [setWidth(int value)](#setWidth-int-) | Представляет ширину фигуры в пикселях. |
| [setWidthCM(double value)](#setWidthCM-double-) | Представляет ширину фигуры в сантиметрах. |
| [setWidthInch(double value)](#setWidthInch-double-) | Представляет ширину фигуры в дюймах. |
| [setWidthPt(double value)](#setWidthPt-double-) | Представляет ширину фигуры в пунктах. |
| [setWidthScale(int value)](#setWidthScale-int-) | Устанавливает масштаб ширины в процентах от исходной ширины изображения. |
| [setX(int value)](#setX-int-) | Устанавливает горизонтальное смещение фигуры от левого края листа в пикселях. |
| [setY(int value)](#setY-int-) | Устанавливает вертикальное смещение фигуры от верхней границы листа, в пикселях. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Возвращает позицию фигуры в порядке Z. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```


Добавляет гиперссылку к фигуре.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Перемещает изображение в правый верхний угол.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | индекс строки. |
| rightColumn | int | индекс столбца. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Возвращает или задаёт описательную (альтернативную) строку текста объекта [GridShape](../../com.aspose.gridweb/gridshape).

**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Представляет [Color](../../com.aspose.cells/color) границы линии изображения.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Получает толщину границы линии изображения в единицах pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях.

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


Получает данные изображения.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Представляет высоту фигуры в пикселях.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Представляет высоту фигуры в дюймах.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Представляет высоту фигуры в дюймах.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Представляет высоту фигуры в пунктах.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Получает масштаб высоты в процентах от исходной высоты изображения. Если объект не является изображением, свойство HeightScale возвращает только 100;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Получает HTML-строку, содержащую данные и некоторые форматирования в этом текстовом поле.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Получает гиперссылку фигуры.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


Получает/устанавливает ID изображения.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Получает формат изображения.

Смотрите [GridImageType](../../com.aspose.gridweb/gridimagetype).

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Представляет горизонтальное смещение фигуры от её левого столбца в пикселях.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Представляет горизонтальное смещение фигуры от её левого столбца в дюймах.

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Представляет горизонтальное смещение фигуры от левого края листа, в пикселях.

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Получает диапазон листа, связанный со значением элемента управления.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Получает горизонтальное смещение фигуры от её столбца нижнего правого угла. Диапазон значения от 0 до 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Получает вертикальное смещение фигуры от её строки нижнего правого угла. Диапазон значения от 0 до 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Представляет индекс столбца нижнего правого угла.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Представляет индекс строки нижнего правого угла.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя фигуры.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Получает исходную высоту изображения.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Получает исходную высоту изображения в сантиметрах.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Получает исходную высоту изображения в дюймах.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Получает исходную ширину изображения.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Получает исходную ширину изображения в сантиметрах.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Получает исходную ширину изображения в дюймах.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Указывает, является ли фигура относительной к оригинальному размеру изображения.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Получает вращение фигуры.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Получает путь и имя исходного файла для связанного изображения.

**Remarks**

Значение по умолчанию — пустая строка. Если SourceFullName не пустая строка, изображение будет связано. Если SourceFullName не пустая строка, но Data равно null, тогда изображение связано и не сохраняется в файле.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Представляет строку в этом объекте TextBox.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Указывает заголовок (подпись) текущего объекта фигуры.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Представляет вертикальное смещение фигуры от её верхней строки, в пикселях.

**Remarks**

Если форма находится в диаграмме, представляет вертикальное смещение формы от её верхней границы.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Представляет вертикальное смещение фигуры от её верхней строки, в дюймах.

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях.

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Получает горизонтальное смещение фигуры от её столбца верхнего левого угла. Диапазон значения от 0 до 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Получает вертикальное смещение фигуры от её строки верхнего левого угла. Диапазон значения от 0 до 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Представляет индекс столбца левого верхнего угла.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Представляет индекс строки верхнего левого угла.

**Remarks**

Если форма находится в другой форме или в группе, UpperLeftRow будет игнорироваться.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Представляет ширину фигуры в пикселях.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Представляет ширину фигуры в сантиметрах.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Представляет ширину фигуры в дюймах.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Представляет ширину фигуры в пунктах.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Получает масштаб ширины в процентах от исходной ширины изображения. Если объект не является изображением, свойство WidthScale возвращает только 100;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Получает горизонтальное смещение фигуры от левого края листа, в пикселях.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Получает вертикальное смещение фигуры от верхнего края листа в пикселях.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Возвращает позицию фигуры в порядке Z.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Получает, видима ли линия границы фигуры.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Получает, отражена ли фигура по вертикали.

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Указывает, является ли фигура группой.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Указывает, видим ли объект.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True означает, что изменения соотношения сторон не допускаются.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True, если объект заблокирован, False, если объект может быть изменён, когда лист защищён.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Получает тип переноса текста у объекта, содержащего текст.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Перемещает изображение в указанное место.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | int | Индекс строки в верхнем левом углу. |
| upperLeftColumn | int | Индекс столбца в верхнем левом углу. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Перемещает объект в указанный диапазон.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftRow | int | Индекс строки в верхнем левом углу. |
| upperLeftColumn | int | Индекс столбца в верхнем левом углу. |
| lowerRightRow | int | Индекс строки в нижнем правом углу |
| lowerRightColumn | int | Индекс столбца в нижнем правом углу |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Удалить гиперссылку фигуры.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Создаёт изображение и сохраняет его в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Возвращает или задаёт описательную (альтернативную) строку текста объекта [GridShape](../../com.aspose.gridweb/gridshape).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


Представляет [Color](../../com.aspose.cells/color) границы линии изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Устанавливает толщину границы изображения в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Получает данные изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Устанавливает, будет ли объект отражён по вертикали.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Устанавливает видимость границы линии объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Представляет высоту фигуры в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Представляет высоту фигуры в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Представляет высоту фигуры в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Представляет высоту фигуры в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Устанавливает масштаб высоты в процентах от исходной высоты изображения. Если фигура не является изображением, свойство HeightScale возвращает только 100;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Указывает, видим ли объект.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Устанавливает HTML‑строку, содержащую данные и некоторые форматирования, в этом текстовом поле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Получает/устанавливает ID изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


Представляет горизонтальное смещение фигуры от её левого столбца в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Представляет горизонтальное смещение фигуры от её левого столбца в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Представляет горизонтальное смещение фигуры от левого края листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Устанавливает диапазон листа, связанный со значением элемента управления.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True означает, что изменения соотношения сторон не допускаются.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True, если объект заблокирован, False, если объект может быть изменён, когда лист защищён.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Устанавливает горизонтальное смещение фигуры от её столбца нижнего правого угла. Диапазон значения от 0 до 1024.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Устанавливает вертикальное смещение фигуры от её строки нижнего правого угла. Диапазон значения от 0 до 256.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Представляет индекс столбца нижнего правого угла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Представляет индекс строки нижнего правого угла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Указывает, является ли фигура относительной к оригинальному размеру изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Устанавливает вращение объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Устанавливает путь и имя исходного файла для связанного изображения.

**Remarks**

Значение по умолчанию — пустая строка. Если SourceFullName не пустая строка, изображение будет связано. Если SourceFullName не пустая строка, но Data равно null, тогда изображение связано и не сохраняется в файле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Представляет строку в этом объекте TextBox.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Устанавливает тип переноса текста в фигуре, содержащей текст.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Указывает заголовок (подпись) текущего объекта фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Представляет вертикальное смещение фигуры от её верхней строки, в пикселях.

**Remarks**

Если форма находится в диаграмме, представляет вертикальное смещение формы от её верхней границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Представляет вертикальное смещение фигуры от её верхней строки, в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Представляет вертикальное смещение фигуры от верхнего края листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Устанавливает горизонтальное смещение фигуры от её столбца верхнего левого угла. Диапазон значения от 0 до 1024.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Устанавливает вертикальное смещение фигуры от её строки верхнего левого угла. Диапазон значения от 0 до 256.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Представляет индекс столбца левого верхнего угла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Представляет индекс строки верхнего левого угла.

**Remarks**

Если форма находится в другой форме или в группе, UpperLeftRow будет игнорироваться.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Представляет ширину фигуры в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Представляет ширину фигуры в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Представляет ширину фигуры в дюймах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Представляет ширину фигуры в пунктах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Устанавливает масштаб ширины в процентах от исходной ширины изображения. Если фигура не является изображением, свойство WidthScale возвращает только 100;

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Устанавливает горизонтальное смещение фигуры от левого края листа в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Устанавливает вертикальное смещение фигуры от верхней границы листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Возвращает позицию фигуры в порядке Z.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

