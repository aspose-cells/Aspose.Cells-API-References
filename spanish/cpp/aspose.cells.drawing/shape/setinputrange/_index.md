---
title: Aspose::Cells::Drawing::Shape::SetInputRange method
linktitle: SetInputRange
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::SetInputRange method. Gets or sets the worksheet range used to fill the specified combo box in C++.'
type: docs
weight: 14800
url: /es/cpp/aspose.cells.drawing/shape/setinputrange/
---
## Shape::SetInputRange(const U16String\&) method


Gets or sets the worksheet range used to fill the specified combo box.

```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const U16String &value)
```


## Examples


```cpp
U16String range = u"$A$1:$A$5";
if (shape.GetInputRange() == u"$B$6:$B10")
    shape.SetInputRange(range);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const char16_t*) method


Gets or sets the worksheet range used to fill the specified combo box.

```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const char16_t *value)
```


## Examples


```cpp
if (shape.GetInputRange() == u"$B$6:$B10")
    shape.SetInputRange(u"$A$1:$A$5");
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const U16String\&, bool, bool) method


Sets the range used to fill the control.

```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const U16String &formula, bool isR1C1, bool isLocal)
```


| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | The range used to fill the control. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |


## Examples


```cpp
//Después de ejecutar el código a continuación, se crea un objeto ListBox en el archivo generado. Cuando se hace clic en la opción seleccionada, el valor seleccionado se muestra en la celda A12.

for (int i = 0; i < 10; ++i)
{
    Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
    cell.PutValue(i + 1);
}

//Crear un objeto ListBox

//Controles ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Controles de formulario
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Establece el rango usado para rellenar el control.
U16String val = u"$A$1:$A$6";
listBox.SetInputRange(val, false, false);

//Establece el rango vinculado al valor del control.
listBox.SetLinkedCell(u"$A$12", false, true);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
## Shape::SetInputRange(const char16_t*, bool, bool) method


Sets the range used to fill the control.

```cpp
void Aspose::Cells::Drawing::Shape::SetInputRange(const char16_t *formula, bool isR1C1, bool isLocal)
```


| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | The range used to fill the control. |
| isR1C1 | bool | Whether the formula needs to be formatted as R1C1. |
| isLocal | bool | Whether the formula needs to be formatted by locale. |


## Examples


```cpp
//Después de ejecutar el código a continuación, se crea un objeto ListBox en el archivo generado. Cuando se hace clic en la opción seleccionada, el valor seleccionado se muestra en la celda A12.

for (int i = 0; i < 10; ++i)
{
    Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
    cell.PutValue(i + 1);
}

//Crear un objeto ListBox

//Controles ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Controles de formulario
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Establece el rango usado para rellenar el control.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Establece el rango vinculado al valor del control.
listBox.SetLinkedCell(u"$A$12", false, true);
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
