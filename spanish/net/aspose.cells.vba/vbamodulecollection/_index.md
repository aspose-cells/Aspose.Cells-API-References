---
title: "Clase VbaModuleCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Vba.VbaModuleCollection. Representa la lista de VbaModule"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/
---
## VbaModuleCollection class

Representa la lista de [`VbaModule`](../vbamodule/)

```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item/) { get; } | Obtiene [`VbaModule`](../vbamodule/) en la lista por el índice. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add_1)(Worksheet) | Agrega módulo para una hoja de cálculo. |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add)(VbaModuleType, string) | Agrega módulo. |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage/)(string, byte[]) |  |
| [AddUserForm](../../aspose.cells.vba/vbamodulecollection/adduserform/)(string, string, byte[]) | Insertar formulario de usuario en el proyecto VBA. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VbaModule[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VbaModule&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VbaModule&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage/)(string) | Representa los datos del Diseñador. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove_1)(string) | Eliminar el módulo por el nombre |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove)(Worksheet) | Elimina módulo para una hoja de cálculo. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaClassVbaModuleCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar un nuevo módulo de clase
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestClass");
            
            // Obtener el módulo añadido y agregar algo de código
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Public Sub TestMethod()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
            
            // Guardar como libro de trabajo habilitado para macros
            workbook.Save("VbaModuleCollectionDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


