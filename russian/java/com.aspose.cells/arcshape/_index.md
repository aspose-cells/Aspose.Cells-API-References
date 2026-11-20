---
title: "ArcShape"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет форму дуги."
type: docs
url: /ru/java/com.aspose.cells/arcshape/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class ArcShape extends Shape
```

Представляет форму дуги.

**Example**

```
         //Instantiate a new Workbook.
         Workbook excelbook = new Workbook();
 
         //Add an arc shape.
         ArcShape arc1 = excelbook.getWorksheets().get(0).getShapes().addArc(2, 0, 2, 0, 130, 130);
 
         //Set the placement of the arc.
         arc1.setPlacement(PlacementType.FREE_FLOATING);
 
         //Set the fill format.
         arc1.getFill().setFillType(FillType.SOLID);
         arc1.getFill().getSolidFill().setColor(Color.getBlue());
 
         //Set the line style.
         arc1.getLine().setCompoundType(MsoLineStyle.SINGLE);
 
         //Set the line weight.
         arc1.getLine().setWeight(2);
 
         //Set the color of the arc line.
         arc1.getLine().setFillType(FillType.SOLID);
         arc1.getLine().getSolidFill().setColor(Color.getRed());
 
         //Set the dash style of the arc.
         arc1.getLine().setDashStyle(MsoLineDashStyle.SOLID);
 
         //Add another arc shape.
         ArcShape arc2 = excelbook.getWorksheets().get(0).getShapes().addArc(9, 0, 2, 0, 130, 130);
 
         //Set the placement of the arc.
         arc2.setPlacement(PlacementType.FREE_FLOATING);
 
         //Set the line style.
         arc2.getLine().setCompoundType(MsoLineStyle.SINGLE);
 
         //Set the line weight.
         arc2.getLine().setWeight(1);
 
         //Set the color of the arc line.
         arc2.getLine().setFillType(FillType.SOLID);
         arc2.getLine().getSolidFill().setColor(Color.getBlue());
 
         //Set the dash style of the arc.
         arc2.getLine().setDashStyle(MsoLineDashStyle.SOLID);
 
         //Save the excel file.
         excelbook.save("tstarcs.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Добавляет гиперссылку к фигуре. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Перемещает изображение в правый верхний угол. |
| [calculateTextSize()](#calculateTextSize--) | Пересчитать область текста |
| [characters(int startIndex, int length)](#characters-int-int-) | Возвращает объект Characters, представляющий диапазон символов в тексте. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fitToTextSize()](#fitToTextSize--) | Пересчитывает область текста, подходящую для отображения всего содержимого. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Форматирует некоторые символы с помощью настройки шрифта. |
| [getActiveXControl()](#getActiveXControl--) | Получает элемент управления ActiveX. |
| [getActualBox()](#getActualBox--) | Получить фактическое положение и размер фигуры (после применения вращения, отражения и т.д.) |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Получить фактическую нижнюю строку. |
| [getAlternativeText()](#getAlternativeText--) | Возвращает или задает описательную (альтернативную) строку текста объекта [Shape](../../com.aspose.cells/shape). |
| [getAnchorType()](#getAnchorType--) | Получает тип заполнителя привязки фигуры. |
| [getAutoShapeType()](#getAutoShapeType--) | Получает тип автофигуры. |
| [getBottom()](#getBottom--) | Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях. |
| [getCharacters()](#getCharacters--) | Возвращает все объекты Characters, представляющие диапазон символов в тексте. |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Получить точки соединения |
| [getControlData()](#getControlData--) | Получает данные элемента управления. |
| [getCreateId()](#getCreateId--) | Получает идентификатор создания этой фигуры. |
| [getFill()](#getFill--) | Возвращает объект [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) , содержащий свойства заливки для указанной фигуры. |
| [getFillFormat()](#getFillFormat--) | Возвращает объект MsoFillFormat, содержащий свойства заливки для указанной фигуры. |
| [getFont()](#getFont--) | Представляет шрифт фигуры. |
| [getFormatPicture()](#getFormatPicture--) | Получает параметры формата изображения. |
| [getGeometry()](#getGeometry--) | Получает геометрию |
| [getGlow()](#getGlow--) | Представляет объект [GlowEffect](../../com.aspose.cells/gloweffect), задающий эффект свечения для элемента диаграммы или фигуры. |
| [getGroup()](#getGroup--) | Получает групповую фигуру, содержащую эту фигуру. |
| [getHeight()](#getHeight--) | Представляет высоту фигуры в пикселях. |
| [getHeightCM()](#getHeightCM--) | Представляет высоту фигуры в сантиметрах. |
| [getHeightInShape()](#getHeightInShape--) | Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры. |
| [getHeightInch()](#getHeightInch--) | Представляет высоту фигуры в дюймах. |
| [getHeightPt()](#getHeightPt--) | Представляет высоту фигуры в пунктах. |
| [getHeightScale()](#getHeightScale--) | Получает масштаб высоты в процентах от исходной высоты изображения. |
| [getHtmlText()](#getHtmlText--) | Получает HTML-строку, содержащую данные и некоторые форматы в этом текстовом поле. |
| [getHyperlink()](#getHyperlink--) | Получает гиперссылку фигуры. |
| [getId()](#getId--) | Получает идентификатор этой фигуры. |
| [getInputRange()](#getInputRange--) | Получает диапазон листа, используемый для заполнения указанного комбинированного списка. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Получает диапазон, используемый для заполнения элемента управления. |
| [getLeft()](#getLeft--) | Представляет горизонтальное смещение фигуры от её левого столбца в пикселях. |
| [getLeftCM()](#getLeftCM--) | Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах. |
| [getLeftInShape()](#getLeftInShape--) | Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры. |
| [getLeftInch()](#getLeftInch--) | Представляет горизонтальное смещение фигуры от её левого столбца в дюймах. |
| [getLeftToCorner()](#getLeftToCorner--) | Получает горизонтальное смещение фигуры от левой границы листа. |
| [getLine()](#getLine--) | Получает стиль линии. |
| [getLineFormat()](#getLineFormat--) | Возвращает объект MsoLineFormat, содержащий свойства форматирования линии для указанной фигуры. |
| [getLinkedCell()](#getLinkedCell--) | Получает диапазон листа, связанный со значением элемента управления. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Получает диапазон, связанный со значением элемента управления. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Получает значение свойства locked. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Получает горизонтальное смещение фигуры от столбца её нижнего правого угла. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Получает вертикальное смещение фигуры от строки её нижнего правого угла. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Представляет индекс столбца нижнего правого угла. |
| [getLowerRightRow()](#getLowerRightRow--) | Представляет индекс строки нижнего правого угла. |
| [getMacroName()](#getMacroName--) | Получает имя макроса. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Получает тип рисунка. |
| [getName()](#getName--) | Получает имя фигуры. |
| [getPaths()](#getPaths--) | Получает пути пользовательской геометрической фигуры. |
| [getPlacement()](#getPlacement--) | Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. |
| [getReflection()](#getReflection--) | Представляет объект [ReflectionEffect](../../com.aspose.cells/reflectioneffect), определяющий эффект отражения для элемента диаграммы или фигуры. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Указывает, является ли фигура относительной к оригинальному размеру изображения. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Преобразование SmartArt в сгруппированные фигуры. |
| [getRichFormattings()](#getRichFormattings--) | Возвращает все объекты Characters, представляющие диапазон символов в тексте. |
| [getRight()](#getRight--) | Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях. |
| [getRotationAngle()](#getRotationAngle--) | Получает вращение фигуры. |
| [getShadowEffect()](#getShadowEffect--) | Представляет объект [ShadowEffect](../../com.aspose.cells/shadoweffect), определяющий эффект тени для элемента диаграммы или фигуры. |
| [getSoftEdges()](#getSoftEdges--) | Получает радиус размытия, применяемый к краям, в единицах точек. |
| [getSpid()](#getSpid--) | Указывает необязательный строковый идентификатор, который приложение может использовать для идентификации конкретной фигуры. |
| [getSpt()](#getSpt--) | Указывает необязательное число, которое приложение может использовать для связывания конкретной фигуры с определённым типом фигуры. |
| [getText()](#getText--) | Получает текст этой фигуры. |
| [getTextBody()](#getTextBody--) | Получает настройку текста фигуры. |
| [getTextBoxOptions()](#getTextBoxOptions--) | Получает текстовую информацию в фигуре |
| [getTextDirection()](#getTextDirection--) | Получает направление потока текста для этого объекта. |
| [getTextEffect()](#getTextEffect--) | Возвращает объект TextEffectFormat, содержащий свойства форматирования текстовых эффектов для указанной фигуры. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Получает тип горизонтального выравнивания текста фигуры. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Получает тип горизонтального переполнения текста в фигуре, содержащей текст. |
| [getTextOptions()](#getTextOptions--) | Представляет параметры текста фигуры. |
| [getTextOrientationType()](#getTextOrientationType--) | Получает тип ориентации текста фигуры. |
| [getTextShapeType()](#getTextShapeType--) | Получает тип предустановленной текстовой фигуры. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Получает тип вертикального выравнивания текста фигуры. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Получает тип вертикального переполнения текста в фигуре, содержащей текст. |
| [getThreeDFormat()](#getThreeDFormat--) | Получает 3D-формат фигуры. |
| [getTitle()](#getTitle--) | Указывает заголовок (подпись) текущего объекта фигуры. |
| [getTop()](#getTop--) | Представляет вертикальное смещение фигуры от её верхней строки, в пикселях. |
| [getTopCM()](#getTopCM--) | Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах. |
| [getTopInShape()](#getTopInShape--) | Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры. |
| [getTopInch()](#getTopInch--) | Представляет вертикальное смещение фигуры от её верхней строки, в дюймах. |
| [getTopToCorner()](#getTopToCorner--) | Получает вертикальное смещение фигуры от верхней границы листа, в пикселях. |
| [getType()](#getType--) | Получает тип автофигуры. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Получает горизонтальное смещение фигуры от её столбца в левом верхнем углу. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Получает вертикальное смещение фигуры от её строки в левом верхнем углу. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Представляет индекс столбца левого верхнего угла. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Представляет индекс верхней строки. |
| [getWidth()](#getWidth--) | Представляет ширину фигуры в пикселях. |
| [getWidthCM()](#getWidthCM--) | Представляет ширину фигуры в сантиметрах. |
| [getWidthInShape()](#getWidthInShape--) | Представляет ширину фигуры в единицах 1/4000 от родительской фигуры. |
| [getWidthInch()](#getWidthInch--) | Представляет ширину фигуры в дюймах. |
| [getWidthPt()](#getWidthPt--) | Представляет ширину фигуры в пунктах. |
| [getWidthScale()](#getWidthScale--) | Получает масштаб ширины в процентах от исходной ширины изображения. |
| [getWorksheet()](#getWorksheet--) | Получает объект [Worksheet](../../com.aspose.cells/worksheet), содержащий эту фигуру. |
| [getX()](#getX--) | Получает горизонтальное смещение фигуры от левого края листа в пикселях. |
| [getY()](#getY--) | Получает вертикальное смещение фигуры от верхнего края листа в пикселях. |
| [getZOrderPosition()](#getZOrderPosition--) | Возвращает позицию фигуры в порядке Z. |
| [hasLine()](#hasLine--) | Получает, видима ли линия границы фигуры. |
| [hashCode()](#hashCode--) |  |
| [isAspectRatioLocked()](#isAspectRatioLocked--) | True означает, что соотношение сторон фигуры заблокировано. |
| [isDecorative()](#isDecorative--) | Указывает, является ли объект декоративным. |
| [isEquation()](#isEquation--) | Указывает, содержит ли фигура только уравнение. |
| [isFilled()](#isFilled--) | Указывает, видим ли формат заливки. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Получает, отражена ли фигура по горизонтали. |
| [isFlippedVertically()](#isFlippedVertically--) | Получает, отражена ли фигура по вертикали. |
| [isGroup()](#isGroup--) | Указывает, является ли эта фигура групповой. |
| [isHidden()](#isHidden--) | Указывает, видим ли объект. |
| [isInGroup()](#isInGroup--) | Указывает, сгруппирована ли фигура. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True означает, что соотношение сторон фигуры заблокировано. |
| [isLocked()](#isLocked--) | True означает, что объект нельзя изменить, когда лист защищён. |
| [isPrintable()](#isPrintable--) | Указывает, печатается ли объект. |
| [isRichText()](#isRichText--) | Является ли текст форматированным. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Возвращает, одинаковы ли фигуры. |
| [isSmartArt()](#isSmartArt--) | Указывает, является ли объект смарт-артом. |
| [isTextWrapped()](#isTextWrapped--) | Получает тип переноса текста у объекта, содержащего текст. |
| [isWordArt()](#isWordArt--) | Указывает, является ли данный объект ворд-артом. |
| [moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)](#moveToRange-int-int-int-int-) | Перемещает объект в указанный диапазон. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Удалить элемент управления ActiveX. |
| [removeHyperlink()](#removeHyperlink--) | Удаляет гиперссылку объекта. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Возвращает или задает описательную (альтернативную) строку текста объекта [Shape](../../com.aspose.cells/shape). |
| [setAnchorType(int value)](#setAnchorType-int-) | Устанавливает тип заполняющего места привязки объекта. |
| [setAspectRatioLocked(boolean value)](#setAspectRatioLocked-boolean-) | True означает, что соотношение сторон фигуры заблокировано. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Устанавливает тип автофигуры. |
| [setBottom(int value)](#setBottom-int-) | Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Устанавливает идентификатор создания для этого объекта. |
| [setDecorative(boolean value)](#setDecorative-boolean-) | Указывает, является ли объект декоративным. |
| [setFilled(boolean value)](#setFilled-boolean-) | Указывает, видим ли формат заливки. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Устанавливает, будет ли объект отражён по горизонтали. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Устанавливает, будет ли объект отражён по вертикали. |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Представляет шрифт фигуры. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Устанавливает видимость границы линии объекта. |
| [setHeight(int value)](#setHeight-int-) | Представляет высоту фигуры в пикселях. |
| [setHeightCM(double value)](#setHeightCM-double-) | Представляет высоту фигуры в сантиметрах. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры. |
| [setHeightInch(double value)](#setHeightInch-double-) | Представляет высоту фигуры в дюймах. |
| [setHeightPt(double value)](#setHeightPt-double-) | Представляет высоту фигуры в пунктах. |
| [setHeightScale(int value)](#setHeightScale-int-) | Устанавливает масштаб высоты в процентах от исходной высоты изображения. |
| [setHidden(boolean value)](#setHidden-boolean-) | Указывает, видим ли объект. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Устанавливает HTML‑строку, содержащую данные и некоторые форматы в этом текстовом поле. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Устанавливает диапазон листа, используемый для заполнения указанного комбобокса. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Устанавливает диапазон, используемый для заполнения элемента управления. |
| [setLeft(int value)](#setLeft-int-) | Представляет горизонтальное смещение фигуры от её левого столбца в пикселях. |
| [setLeftCM(double value)](#setLeftCM-double-) | Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры. |
| [setLeftInch(double value)](#setLeftInch-double-) | Представляет горизонтальное смещение фигуры от её левого столбца в дюймах. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Устанавливает горизонтальное смещение объекта от левого края листа. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Устанавливает диапазон листа, связанный со значением элемента управления. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Устанавливает диапазон, связанный со значением элемента управления. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True означает, что соотношение сторон фигуры заблокировано. |
| [setLocked(boolean value)](#setLocked-boolean-) | True означает, что объект нельзя изменить, когда лист защищён. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Установите свойство блокировки. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Устанавливает горизонтальное смещение объекта от столбца его нижнего правого угла. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Устанавливает вертикальное смещение объекта от строки его нижнего правого угла. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Представляет индекс столбца нижнего правого угла. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Представляет индекс строки нижнего правого угла. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Устанавливает имя макроса. |
| [setName(String value)](#setName-java.lang.String-) | Устанавливает имя объекта. |
| [setPlacement(int value)](#setPlacement-int-) | Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | Указывает, печатается ли объект. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Указывает, является ли фигура относительной к оригинальному размеру изображения. |
| [setRight(int value)](#setRight-int-) | Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Устанавливает вращение объекта. |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Устанавливает радиус размытия, применяемый к краям, в единицах точек. |
| [setText(String value)](#setText-java.lang.String-) | Устанавливает текст этой фигуры. |
| [setTextDirection(int value)](#setTextDirection-int-) | Устанавливает направление потока текста для этого объекта. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Устанавливает тип горизонтального выравнивания текста фигуры. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Устанавливает тип горизонтального переполнения текста в фигуре, содержащей текст. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Представляет параметры текста фигуры. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Устанавливает тип ориентации текста фигуры. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Устанавливает предустановленный тип текстовой фигуры. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Устанавливает тип вертикального выравнивания текста фигуры. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Устанавливает тип вертикального переполнения текста в фигуре, содержащей текст. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Устанавливает тип переноса текста в фигуре, содержащей текст. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Указывает заголовок (подпись) текущего объекта фигуры. |
| [setTop(int value)](#setTop-int-) | Представляет вертикальное смещение фигуры от её верхней строки, в пикселях. |
| [setTopCM(double value)](#setTopCM-double-) | Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах. |
| [setTopInShape(int value)](#setTopInShape-int-) | Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры. |
| [setTopInch(double value)](#setTopInch-double-) | Представляет вертикальное смещение фигуры от её верхней строки, в дюймах. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Устанавливает вертикальное смещение фигуры от верхней границы листа, в пикселях. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Устанавливает горизонтальное смещение фигуры от столбца её верхнего левого угла. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Устанавливает вертикальное смещение фигуры от строки её верхнего левого угла. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Представляет индекс столбца левого верхнего угла. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Представляет индекс верхней строки. |
| [setWidth(int value)](#setWidth-int-) | Представляет ширину фигуры в пикселях. |
| [setWidthCM(double value)](#setWidthCM-double-) | Представляет ширину фигуры в сантиметрах. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Представляет ширину фигуры в единицах 1/4000 от родительской фигуры. |
| [setWidthInch(double value)](#setWidthInch-double-) | Представляет ширину фигуры в дюймах. |
| [setWidthPt(double value)](#setWidthPt-double-) | Представляет ширину фигуры в пунктах. |
| [setWidthScale(int value)](#setWidthScale-int-) | Устанавливает масштаб ширины в процентах от исходной ширины изображения. |
| [setX(int value)](#setX-int-) | Устанавливает горизонтальное смещение фигуры от левой границы листа, в пикселях. |
| [setY(int value)](#setY-int-) | Устанавливает вертикальное смещение фигуры от верхней границы листа, в пикселях. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Возвращает позицию фигуры в порядке Z. |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Перемещает фигуру на передний план или отправляет её на задний план. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Создаёт изображение фигуры и сохраняет его в поток в указанном формате. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Сохраняет фигуру в поток. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Сохраняет фигуру в файл. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Обновляет выбранное значение значением связанной ячейки. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Добавляет гиперссылку к фигуре.

**Example**

```
         Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| адрес | java.lang.String | Адрес гиперссылки. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Returns the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Перемещает изображение в правый верхний угол.

**Example**

```
         shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | индекс строки. |
| rightColumn | int | индекс столбца. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Пересчитать область текста

**Example**

```
         //The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Размер текста в массиве (ширина и высота).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Возвращает объект Characters, представляющий диапазон символов в тексте.

**Remarks**

Этот метод работает только с фигурой, у которой есть заголовок.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Индекс начала символа. |
| length | int | Количество символов. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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
### fitToTextSize() {#fitToTextSize--}
```
public void fitToTextSize()
```


Пересчитывает область текста, подходящую для отображения всего содержимого.

**Example**

```
         if (shape.getName().startsWith("Your traget"))
         {
             shape.fitToTextSize();
         }
```

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Форматирует некоторые символы с помощью настройки шрифта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| startIndex | int | Начальный индекс. |
| length | int | Длина. |
| font | [Font](../../com.aspose.cells/font) | Настройка шрифта. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Флаг настройки шрифта. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Получает элемент управления ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
             //The font name of CheckBox
             String fontName = checkBox1.getFont().getName();
         }
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualBox() {#getActualBox--}
```
public float[] getActualBox()
```


Получить фактическое положение и размер фигуры (после применения вращения, отражения и т.д.)

**Remarks**

Примечание: Интерфейс не полностью функционален, особенно информация о местоположении некорректна. Рекомендуется не использовать этот интерфейс, пока функция не будет завершена.

**Example**

```
         float[] box = shape.getActualBox();
         System.out.println("x = " + box[0]);
         System.out.println("y = " + box[1]);
         System.out.println("w = " + box[2]);
         System.out.println("h = " + box[3]);
```

**Returns:**
float[] - Возвращает позицию и размер в порядке x, y, w, h.
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Получить фактическую нижнюю строку.

**Example**

```
         int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Возвращает или задает описательную (альтернативную) строку текста объекта [Shape](../../com.aspose.cells/shape).

**Example**

```
         shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


Получает тип заполнителя привязки фигуры.

См. [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

```
         if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


Получает тип автофигуры.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях.

**Example**

```
         if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Возвращает все объекты Characters, представляющие диапазон символов в тексте.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Shape.GetRichFormattings(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         FontSetting fontSetting = shape.characters(0, 4);
```

**Returns:**
java.util.ArrayList - Все объекты Characters.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Получить точки соединения

**Example**

```
         float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - Пары [X,Y] точки соединения. Каждый элемент представляет собой массив float[2], где [0] — x, а [1] — y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Получает данные элемента управления.

**Example**

```
         if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


Получает идентификатор создания этой фигуры.

**Example**

```
         System.out.println(shape.getCreateId());
         java.util.UUID g = java.util.UUID.randomUUID();
         shape.setCreateId(g);
         System.out.println(shape.getCreateId());
```

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Возвращает объект [getFillFormat()](../../com.aspose.cells/shape\#getFillFormat--) , содержащий свойства заливки для указанной фигуры.

**Example**

```
         FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


Возвращает объект MsoFillFormat, содержащий свойства заливки для указанной фигуры.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство Shape.Fill. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Представляет шрифт фигуры.

**Example**

```
         Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


Получает параметры формата изображения.

**Example**

```
         MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Получает геометрию

**Example**

```
         if (shape.getGeometry() != null &&shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


Представляет объект [GlowEffect](../../com.aspose.cells/gloweffect), задающий эффект свечения для элемента диаграммы или фигуры.

**Example**

```
         GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


Получает групповую фигуру, содержащую эту фигуру.

**Example**

```
         GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Представляет высоту фигуры в пикселях.

**Example**

```
         if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Представляет высоту фигуры в сантиметрах.

**Example**

```
         if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Example**

```
         if (shape.isInGroup() &&shape.getHeightInShape() == 4000)
             shape.setHeightInShape(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Представляет высоту фигуры в дюймах.

**Example**

```
         if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Представляет высоту фигуры в пунктах.

**Example**

```
         if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


Получает масштаб высоты в процентах от исходной высоты изображения. Если объект не является изображением, свойство HeightScale возвращает только 100;

**Example**

```
         if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


Получает HTML-строку, содержащую данные и некоторые форматы в этом текстовом поле.

**Example**

```
         String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


Получает гиперссылку фигуры.

**Example**

```
         Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


Получает идентификатор этой фигуры.

**Example**

```
         int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Получает диапазон листа, используемый для заполнения указанного комбинированного списка.

**Example**

```
         if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


Получает диапазон, используемый для заполнения элемента управления.

**Example**

```
         String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Диапазон, используемый для заполнения элемента управления.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Представляет горизонтальное смещение фигуры от её левого столбца в пикселях.

**Example**

```
         if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Представляет горизонтальное смещение фигуры от её левого столбца в сантиметрах.

**Example**

```
         if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Example**

```
         if (shape.isInGroup() &&shape.getLeftInShape() == 2000)
             shape.setLeftInShape(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Представляет горизонтальное смещение фигуры от её левого столбца в дюймах.

**Example**

```
         if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Получает горизонтальное смещение фигуры от левой границы листа.

**Example**

```
         if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


Получает стиль линии.

**Example**

```
         LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


Возвращает объект MsoLineFormat, содержащий свойства форматирования линии для указанной фигуры.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Shape.Line. Это свойство будет удалено через 12 месяцев, начиная с июля 2016 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Получает диапазон листа, связанный со значением элемента управления.

**Example**

```
         if (shape.getLinkedCell().equals("$B$6"))
         {
             shape.setLinkedCell("A1");
         }
         shape.updateSelectedValue();
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


Получает диапазон, связанный со значением элемента управления.

**Example**

```
         //You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

**Returns:**
java.lang.String - Диапазон, связанный со значением элемента управления.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Получает значение свойства locked.

**Example**

```
         int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Тип свойства блокировки формы. |

**Returns:**
boolean - Возвращает значение свойства locked.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Получает горизонтальное смещение фигуры от столбца её нижнего правого угла.

**Remarks**

Диапазон значений от 0 до 1024.

**Example**

```
         if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


Получает вертикальное смещение фигуры от строки её нижнего правого угла.

**Remarks**

Диапазон значений от 0 до 256.

**Example**

```
         if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Представляет индекс столбца нижнего правого угла.

**Example**

```
         if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Представляет индекс строки нижнего правого угла.

**Example**

```
         if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


Получает имя макроса.

**Example**

```
         //Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Получает тип рисунка.

См. [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
         /*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя фигуры.

**Example**

```
         shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Получает пути пользовательской геометрической фигуры.

**Example**

```
         //Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Example**

```
         if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Представляет объект [ReflectionEffect](../../com.aspose.cells/reflectioneffect), определяющий эффект отражения для элемента диаграммы или фигуры.

**Example**

```
         ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Указывает, является ли фигура относительной к оригинальному размеру изображения.

**Example**

```
         if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


Преобразование SmartArt в сгруппированные фигуры.

**Example**

```
         if(shape.isSmartArt())
         {
             GroupShape groupShape = shape.getResultOfSmartArt();
         }
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRichFormattings() {#getRichFormattings--}
```
public FontSetting[] getRichFormattings()
```


Возвращает все объекты Characters, представляющие диапазон символов в тексте.

**Example**

```
         FontSetting[] list = shape.getRichFormattings();
```

**Returns:**
com.aspose.cells.FontSetting[] - Все объекты Characters
### getRight() {#getRight--}
```
public int getRight()
```


Представляет ширину горизонтального смещения фигуры от столбца её нижнего правого угла в пикселях.

**Example**

```
         if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Получает вращение фигуры.

**Example**

```
         //Gets rotation angle of the shape.
         double angle = shape.getRotationAngle() ;
 
         //Gets rotation angle of the shape.
          shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Представляет объект [ShadowEffect](../../com.aspose.cells/shadoweffect), определяющий эффект тени для элемента диаграммы или фигуры.

**Example**

```
         ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


Получает радиус размытия, применяемый к краям, в единицах точек.

**Example**

```
         shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


Указывает необязательный строковый идентификатор, который приложение может использовать для идентификации конкретной фигуры.

**Example**

```
         String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


Указывает необязательное число, которое приложение может использовать для связывания конкретной фигуры с определённым типом фигуры.

**Example**

```
         int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Получает текст этой фигуры.

**Example**

```
         if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


Получает настройку текста фигуры.

**Example**

```
         FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextBoxOptions() {#getTextBoxOptions--}
```
public TextBoxOptions getTextBoxOptions()
```


Получает текстовую информацию в фигуре

**Example**

```
         TextBoxOptions textBoxOpt = shape.getTextBoxOptions();
         textBoxOpt.setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
         textBoxOpt.setTopMarginPt(0.2d);
         textBoxOpt.setLeftMarginPt(0.2d);
         textBoxOpt.setRightMarginPt(0.2d);
         textBoxOpt.setBottomMarginPt(0.2d);
```

**Returns:**
[TextBoxOptions](../../com.aspose.cells/textboxoptions)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Получает направление потока текста для этого объекта.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

```
         if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


Возвращает объект TextEffectFormat, содержащий свойства форматирования текстовых эффектов для указанной формы. Применяется к объектам Shape, представляющим WordArt.

**Example**

```
         if(shape.isWordArt())
         {
             TextEffectFormat textEffectFormat = shape.getTextEffect();
         }
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Получает тип горизонтального выравнивания текста фигуры.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Получает тип горизонтального переполнения текста в фигуре, содержащей текст.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Представляет параметры текста фигуры.

**Example**

```
         TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


Получает тип ориентации текста фигуры.

См. [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

```
         if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Получает тип предустановленной текстовой фигуры.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Получает тип вертикального выравнивания текста фигуры.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

```
         if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


Получает тип вертикального переполнения текста в фигуре, содержащей текст.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


Получает 3D-формат фигуры.

**Example**

```
         ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


Указывает заголовок (подпись) текущего объекта фигуры.

**Example**

```
         shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Представляет вертикальное смещение фигуры от её верхней строки, в пикселях.

**Remarks**

Если форма находится в диаграмме, представляет вертикальное смещение формы от её верхней границы.

**Example**

```
         if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Представляет вертикальное смещение фигуры от её верхней строки, в сантиметрах.

**Example**

```
         if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Example**

```
         if (shape.isInGroup() &&shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Представляет вертикальное смещение фигуры от её верхней строки, в дюймах.

**Example**

```
         if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Получает вертикальное смещение фигуры от верхней границы листа, в пикселях.

**Example**

```
         if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Получает тип автофигуры.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         /*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Получает горизонтальное смещение фигуры от её столбца в левом верхнем углу.

**Remarks**

Диапазон значений от 0 до 1024.

**Example**

```
         if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


Получает вертикальное смещение фигуры от её строки в левом верхнем углу.

**Remarks**

Диапазон значений от 0 до 256.

**Example**

```
         if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Представляет индекс столбца левого верхнего угла.

**Example**

```
         if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Представляет индекс верхней строки.

**Remarks**

Если форма находится в другой форме или в группе, UpperLeftRow будет игнорироваться.

**Example**

```
         if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Представляет ширину фигуры в пикселях.

**Example**

```
         if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Представляет ширину фигуры в сантиметрах.

**Example**

```
         if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


Представляет ширину фигуры в единицах 1/4000 от родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Example**

```
         if (shape.isInGroup() &&shape.getWidthInShape() == 2000)
             shape.setWidthInShape(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Представляет ширину фигуры в дюймах.

**Example**

```
         if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Представляет ширину фигуры в пунктах.

**Example**

```
         if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


Получает масштаб ширины в процентах от исходной ширины изображения. Если объект не является изображением, свойство WidthScale возвращает только 100;

**Example**

```
         if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Получает объект [Worksheet](../../com.aspose.cells/worksheet), содержащий эту фигуру.

**Example**

```
         Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


Получает горизонтальное смещение фигуры от левого края листа в пикселях.

**Example**

```
         if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Получает вертикальное смещение фигуры от верхнего края листа в пикселях.

**Example**

```
         if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Возвращает позицию фигуры в порядке Z.

**Example**

```
         shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Получает, видима ли линия границы фигуры.

**Example**

```
         if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAspectRatioLocked() {#isAspectRatioLocked--}
```
public boolean isAspectRatioLocked()
```


True означает, что соотношение сторон фигуры заблокировано.

**Remarks**

Только для изображений и объектов Ole.

**Example**

```
         shape.setAspectRatioLocked(false);
```

**Returns:**
boolean
### isDecorative() {#isDecorative--}
```
public boolean isDecorative()
```


Указывает, является ли объект декоративным.

**Example**

```
         if (!shape.isDecorative())
             shape.setDecorative(true);
```

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Указывает, содержит ли фигура только уравнение.

**Example**

```
         //If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


Указывает, видим ли формат заливки.

**Example**

```
         if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


Получает, отражена ли фигура по горизонтали.

**Example**

```
         if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


Получает, отражена ли фигура по вертикали.

**Example**

```
         if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Указывает, является ли эта фигура групповой.

**Example**

```
         if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Указывает, видим ли объект.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Указывает, сгруппирована ли фигура.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True означает, что соотношение сторон фигуры заблокировано.

**Remarks**

Только для изображений и объектов Ole. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Shape.IsAspectRatioLocked. Это свойство будет удалено через 12 месяцев, начиная с июля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Example**

```
         shape.setHidden(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True означает, что объект нельзя изменить, когда лист защищён. Обратите внимание, что это значение имеет смысл только если лист или объекты на листе защищены.

**Example**

```
         //Sets the specified shape to unlocked state
         if (shape.getWorksheet().isProtected() &&shape.isLocked())
         {
             shape.setLocked(false);
         }
 
         //Sets the specified shape to a locked state
         if (shape.getWorksheet().isProtected() &&!shape.isLocked())
         {
             shape.setLocked(true);
         }
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


Указывает, печатается ли объект. Если False, эта фигура не будет печататься при печати.

**Example**

```
         if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Является ли текст форматированным.

**Example**

```
         if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


Возвращает, одинаковы ли фигуры.

**Example**

```
         if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Указывает, является ли объект смарт-артом.

**Remarks**

Только для файла ooxml.

**Example**

```
         //if true,the shape is a smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Получает тип переноса текста у объекта, содержащего текст.

**Example**

```
         if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


Указывает, является ли данный объект ворд-артом.

**Remarks**

Только для Legacy Shape файла xls.

**Example**

```
         if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```


Перемещает объект в указанный диапазон.

**Example**

```
         shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | int | Индекс строки в верхнем левом углу. |
| leftColumn | int | Индекс столбца в верхнем левом углу. |
| bottomRow | int | Индекс строки в нижнем правом углу |
| rightColumn | int | Индекс столбца в нижнем правом углу |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


Удалить элемент управления ActiveX.

**Example**

```
         if(shape.getActiveXControl() != null)
         {
             shape.removeActiveXControl();
         }
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Удаляет гиперссылку объекта.

**Example**

```
         shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Возвращает или задает описательную (альтернативную) строку текста объекта [Shape](../../com.aspose.cells/shape).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Устанавливает тип заполняющего места привязки объекта.

См. [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setAspectRatioLocked(boolean value) {#setAspectRatioLocked-boolean-}
```
public void setAspectRatioLocked(boolean value)
```


True означает, что соотношение сторон фигуры заблокировано.

**Remarks**

Только для изображений и объектов Ole.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Устанавливает тип автофигуры.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Представляет ширину вертикального смещения фигуры от её нижнего угла, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Устанавливает идентификатор создания для этого объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.UUID |  |

### setDecorative(boolean value) {#setDecorative-boolean-}
```
public void setDecorative(boolean value)
```


Указывает, является ли объект декоративным.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Указывает, видим ли формат заливки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Устанавливает, будет ли объект отражён по горизонтали.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Устанавливает, будет ли объект отражён по вертикали.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Представляет шрифт фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

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


Представляет высоту фигуры в сантиметрах.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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


Устанавливает HTML‑строку, содержащую данные и некоторые форматы в этом текстовом поле.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Устанавливает диапазон листа, используемый для заполнения указанного комбобокса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает диапазон, используемый для заполнения элемента управления.

**Example**

```
         //After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Диапазон, используемый для заполнения элемента управления. |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

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

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Представляет горизонтальное смещение фигуры от левой границы родительской фигуры в единицах 1/4000 ширины родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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


Устанавливает горизонтальное смещение объекта от левого края листа.

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

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Устанавливает диапазон, связанный со значением элемента управления.

**Example**

```
         //After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| formula | java.lang.String | Диапазон, связанный со значением элемента управления. |
| isR1C1 | boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


True означает, что соотношение сторон фигуры заблокировано.

**Remarks**

Только для изображений и объектов Ole. ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Shape.IsAspectRatioLocked. Это свойство будет удалено через 12 месяцев, начиная с июля 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True означает, что объект нельзя изменить, когда лист защищён. Обратите внимание, что это значение имеет смысл только если лист или объекты на листе защищены.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Установите свойство блокировки.

**Example**

```
         shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). Заблокированный тип. |
| значение | boolean | Значение свойства. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Устанавливает горизонтальное смещение объекта от столбца его нижнего правого угла.

**Remarks**

Диапазон значений от 0 до 1024.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Устанавливает вертикальное смещение объекта от строки его нижнего правого угла.

**Remarks**

Диапазон значений от 0 до 256.

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

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Устанавливает имя макроса.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Устанавливает имя объекта.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Представляет способ, которым объект рисунка привязан к находящимся под ним ячейкам. Свойство управляет размещением объекта на листе.

См. [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


Указывает, печатается ли объект. Если False, эта фигура не будет печататься при печати.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Устанавливает радиус размытия, применяемый к краям, в единицах точек.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Устанавливает текст этой фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Устанавливает направление потока текста для этого объекта.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Устанавливает тип горизонтального выравнивания текста фигуры.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Устанавливает тип горизонтального переполнения текста в фигуре, содержащей текст.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Представляет параметры текста фигуры.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Устанавливает тип ориентации текста фигуры.

См. [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Устанавливает предустановленный тип текстовой фигуры.

См. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Устанавливает тип вертикального выравнивания текста фигуры.

См. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Устанавливает тип вертикального переполнения текста в фигуре, содержащей текст.

См. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Представляет вертикальное смещение фигуры от верхней границы родительской фигуры, в единицах 1/4000 высоты родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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


Устанавливает вертикальное смещение фигуры от верхней границы листа, в пикселях.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Устанавливает горизонтальное смещение фигуры от столбца её верхнего левого угла.

**Remarks**

Диапазон значений от 0 до 1024.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Устанавливает вертикальное смещение фигуры от строки её верхнего левого угла.

**Remarks**

Диапазон значений от 0 до 256.

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


Представляет индекс верхней строки.

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

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Представляет ширину фигуры в единицах 1/4000 от родительской фигуры.

**Remarks**

Применяется только когда эта фигура находится в группе или диаграмме.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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


Устанавливает горизонтальное смещение фигуры от левой границы листа, в пикселях.

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

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Перемещает фигуру на передний план или отправляет её на задний план.

**Example**

```
         shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| orders | int | Если значение меньше нуля, перемещает фигуру назад. Если значение больше нуля, перемещает фигуру вперёд. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Создаёт изображение фигуры и сохраняет его в поток в указанном формате.

**Remarks**

Поддерживаются следующие форматы: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream | Поток вывода. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | Формат, в котором сохранять изображение. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Сохраняет фигуру в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Сохраняет фигуру в файл.

**Example**

```
         ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Обновляет выбранное значение значением связанной ячейки.

**Example**

```
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

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

