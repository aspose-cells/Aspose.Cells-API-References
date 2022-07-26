---
title: ColumnCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Colección de laobjetos que representan las columnas individuales configuraciones en una hoja de trabajo. El objeto Columna solo representa configuraciones como el ancho de columna estilos etc. para toda la columna no tiene nada que ver con el hecho de que haya celdas no vacías datos o no en la columna correspondiente. Y el Recuento de esta colección solo representa el recuento de objetos de columna que se han instanciado en este colección no tiene nada que ver con el hecho de que no hay celdas vacías datos o no en la hoja de trabajo.
type: docs
weight: 1070
url: /es/net/aspose.cells/columncollection/
---
## ColumnCollection class

Colección de laobjetos que representan las columnas individuales (configuraciones) en una hoja de trabajo. El objeto Columna solo representa configuraciones como el ancho de columna, estilos, etc. para toda la columna, no tiene nada que ver con el hecho de que haya celdas no vacías (datos) o no en la columna correspondiente. Y el "Recuento" de esta colección solo representa el recuento de objetos de columna que se han instanciado en este colección, no tiene nada que ver con el hecho de que no hay celdas vacías (datos) o no en la hoja de trabajo.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | Obtiene un objeto por índice de columna. El objeto de columna del índice de columna dado se instanciará si no existe antes. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | Obtiene el[`Column`](../column)objeto por la posición en la lista. |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();

//Obteniendo la referencia de la primera hoja de cálculo
Worksheet worksheet = workbook.Worksheets[0];

// Agregar nuevo estilo al libro de trabajo
Style style = workbook.CreateStyle();

//Configurando el color de fondo a Azul
style.ForegroundColor = Color.Blue;

//estableciendo el patrón de fondo
style.Pattern = BackgroundType.Solid;

//Bandera de nuevo estilo
StyleFlag styleFlag = new StyleFlag();

//Establecer todos los estilos
styleFlag.All = true;

//Cambiar el ancho predeterminado de las primeras diez columnas
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

//Obtener la columna con formato no predeterminado
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
    //Aplicar estilo a las primeras diez columnas
    column.ApplyStyle(style, styleFlag);
}

//Guardando el archivo de Excel
workbook.Save("book1.xls");

[VB.NET]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()

'Obtención de la referencia de la primera hoja de cálculo
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Agregar nuevo estilo al libro de trabajo
Dim style As Style = workbook.CreateStyles()

'Establecer el color de fondo en Azul
style.ForegroundColor = Color.Blue

'Configuración del patrón de fondo
style.Pattern = BackgroundType.Solid

'Bandera de nuevo estilo
Dim styleFlag As New StyleFlag()

'Establecer todos los estilos
styleFlag.All = True

'Cambiar el ancho predeterminado de las primeras diez columnas
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Obtenga la columna con formato no predeterminado
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Aplicar estilo a las primeras diez columnas
    column.ApplyStyle(style, styleFlag)
Next column

'Guardar el archivo de Excel
workbook.Save("book1.xls")

```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
