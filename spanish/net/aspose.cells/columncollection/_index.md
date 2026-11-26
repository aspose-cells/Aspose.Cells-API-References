---
title: "Clase ColumnCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ColumnCollection class. Colección de los objetos Column que representan la configuración individual de columnas en una hoja de cálculo. El objeto Column solo representa ajustes como el ancho de columna, estilos, etc., para toda la columna y no tiene relación con el hecho de que haya datos en celdas no vacías o no en la columna correspondiente. Y el Count de esta colección solo representa la cantidad de objetos Column que se han instanciado en esta colección, sin relación con la existencia de datos en celdas no vacías en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/columncollection/
---
## ColumnCollection class

Colección de los objetos [`Column`](../column/) que representan las columnas (configuraciones) individuales en una hoja de cálculo. El objeto Column solo representa ajustes como el ancho de columna, estilos, etc., para toda la columna y no tiene relación con el hecho de que haya celdas no vacías (datos) o no en la columna correspondiente. Y el "Count" de esta colección solo representa la cantidad de objetos Column que se han instanciado en esta colección, sin relación con la existencia de celdas no vacías (datos) en la hoja de cálculo.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Obtiene un objeto [`Column`](../column/) por índice de columna. El objeto Column del índice de columna dado se instanciará si no existe previamente. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsoleto.**) Obtiene el objeto de columna por el índice. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Obtiene el objeto [`Column`](../column/) por la posición en la lista. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar nuevo estilo al libro de trabajo
            Style style = workbook.CreateStyle();

            // Estableciendo el color de fondo a azul
            style.ForegroundColor = Color.Blue;

            // Estableciendo el patrón de fondo
            style.Pattern = BackgroundType.Solid;

            // Nuevo indicador de estilo
            StyleFlag styleFlag = new StyleFlag();

            // Establecer todos los estilos
            styleFlag.All = true;

            // Cambiar el ancho predeterminado de las primeras diez columnas
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Obtener la Column con formato no predeterminado
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Aplicar estilo a las primeras diez Columns
                column.ApplyStyle(style, styleFlag);
            }

            // Guardando el archivo Excel
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


