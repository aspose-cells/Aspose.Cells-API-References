---
title: Replace
second_title: Referencia de API de Aspose.Cells para .NET
description: Reemplaza el valor de una celda con una nueva cadena.
type: docs
weight: 570
url: /es/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

Reemplaza el valor de una celda con una nueva cadena.

```csharp
public int Replace(string placeHolder, string newValue)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValue | String | Valor de cadena para reemplazar |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();
......
workbook.Replace("AnOldValue", "NewValue");

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
 ........
orkbook.Replace("AnOldValue", "NewValue")
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

Reemplaza el valor de una celda con un nuevo entero.

```csharp
public int Replace(string placeHolder, int newValue)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValue | Int32 | Valor entero a reemplazar |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();
......
int newValue = 100;
workbook.Replace("AnOldValue", newValue);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Integer =  100 
orkbook.Replace("AnOldValue", NewValue)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

Reemplaza el valor de una celda con un nuevo doble.

```csharp
public int Replace(string placeHolder, double newValue)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValue | Double | Valor doble para reemplazar |

### Ejemplos

```csharp

[C#]

Workbook workbook = new Workbook();
......
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);


[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Double =  100.0
orkbook.Replace("AnOldValue", NewValue)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

Reemplaza el valor de una celda con una nueva matriz de cadenas.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValues | String[] | Matriz de cadenas para reemplazar |
| isVertical | Boolean | Verdadero - Vertical, Falso - Horizontal |

### Ejemplos

```csharp

[C#]

Workbook workbook = new Workbook();
......
string[] newValues = new string[]{"Tom", "Alice", "Jerry"};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
.............
im NewValues() As String =  New String() {"Tom", "Alice", "Jerry"}		
orkbook.Replace("AnOldValue", NewValues, True)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

Reemplaza los valores de las celdas con una matriz de enteros.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValues | Int32[] | Matriz de enteros a reemplazar |
| isVertical | Boolean | Verdadero - Vertical, Falso - Horizontal |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();
......
int[] newValues = new int[]{1, 2, 3};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
..........
im NewValues() As Integer =  New Integer() {1, 2, 3}
orkbook.Replace("AnOldValue", NewValues, True)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

Reemplaza los valores de las celdas con una matriz doble.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValues | Double[] | Matriz doble para reemplazar |
| isVertical | Boolean | Verdadero - Vertical, Falso - Horizontal |

### Ejemplos

```csharp

[C#]

Workbook workbook = new Workbook();
......
double[] newValues = new double[]{1.23, 2.56, 3.14159};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
...........
Dim NewValues() As Double =  New Double() {1.23, 2.56, 3.14159}
workbook.Replace("AnOldValue", NewValues, True)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

Reemplaza los valores de las celdas con datos de unDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| insertTable | DataTable | Tabla de datos para reemplazar |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// Agrega datos a myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' Agrega datos a myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

Reemplaza los valores de las celdas con nuevos datos.

```csharp
public int Replace(bool boolValue, object newValue)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| boolValue | Boolean | El valor booleano que se va a reemplazar. |
| newValue | Object | Nuevo valor. Puede ser un valor de cadena, entero, doble o de fecha y hora. |

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

Reemplaza los valores de las celdas con nuevos datos.

```csharp
public int Replace(int intValue, object newValue)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| intValue | Int32 | El valor entero que se va a reemplazar. |
| newValue | Object | Nuevo valor. Puede ser un valor de cadena, entero, doble o de fecha y hora. |

### Ver también

* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

Reemplaza el valor de una celda con una nueva cadena.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| placeHolder | String | marcador de posición de celda |
| newValue | String | Valor de cadena para reemplazar |
| options | ReplaceOptions | Las opciones de reemplazo |

### Ver también

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* espacio de nombres [Aspose.Cells](../../workbook)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
