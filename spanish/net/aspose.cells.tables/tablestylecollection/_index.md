---
title: "Clase TableStyleCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Tables.TableStyleCollection. Representa todos los estilos de tabla personalizados."
type: docs
url: /es/net/aspose.cells.tables/tablestylecollection/
---
## TableStyleCollection class

Representa todos los estilos de tabla personalizados.

```csharp
public class TableStyleCollection : CollectionBase<TableStyle>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [DefaultPivotStyleName](../../aspose.cells.tables/tablestylecollection/defaultpivotstylename/) { get; set; } | Obtiene y establece el nombre del estilo predeterminado de la tabla dinámica. |
| [DefaultTableStyleName](../../aspose.cells.tables/tablestylecollection/defaulttablestylename/) { get; set; } | Obtiene y establece el nombre del estilo predeterminado de la tabla. |
| [Item](../../aspose.cells.tables/tablestylecollection/item/) { get; } | Obtiene el estilo de tabla por el índice. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddPivotTableStyle](../../aspose.cells.tables/tablestylecollection/addpivottablestyle/)(string) | Agrega un estilo de tabla dinámica personalizado. |
| [AddTableStyle](../../aspose.cells.tables/tablestylecollection/addtablestyle/)(string) | Agrega un estilo de tabla personalizado. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TableStyle, IComparer&lt;TableStyle&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TableStyle) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TableStyle[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TableStyle[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TableStyle&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TableStyle&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TableStyle&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TableStyle&gt;) |  |
| [GetBuiltinTableStyle](../../aspose.cells.tables/tablestylecollection/getbuiltintablestyle/)(TableStyleType) | Obtiene el estilo de tabla incorporado |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TableStyle, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TableStyle, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Accede a la colección de estilos de tabla
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Muestra los nombres de estilo predeterminados
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Cambia el estilo de tabla predeterminado
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            
            // Guarda el libro de trabajo
            workbook.Save("TableStylesDemo.xlsx");
            
            // Verifica el cambio cargando el archivo guardado
            Workbook verifyWorkbook = new Workbook("TableStylesDemo.xlsx");
            Console.WriteLine("New Default Table Style: " + 
                verifyWorkbook.Worksheets.TableStyles.DefaultTableStyleName);
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TableStyle](../tablestyle/)
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


