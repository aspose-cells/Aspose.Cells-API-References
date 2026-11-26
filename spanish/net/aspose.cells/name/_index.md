---
title: "Clase Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Name. Representa un nombre definido para un rango de celdas"
type: docs
url: /es/net/aspose.cells/name/
---
## Name class

Representa un nombre definido para un rango de celdas.

```csharp
public class Name
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Obtiene y establece el comentario del nombre. Solo se aplica a Excel 2007 o versiones superiores. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Obtiene el texto completo del nombre del objeto con la configuración de alcance. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Indica si este nombre es referenciado por otras fórmulas. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Indica si el nombre es visible. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Obtiene o establece una referencia R1C1 del `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Devuelve o establece la fórmula a la que el nombre está definido para referirse, comenzando con un signo igual. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Indica a qué pertenece este nombre: Libro de trabajo o Hoja de cálculo. 0 = Nombre global, de lo contrario índice a la hoja (basado en uno). |
| [Text](../../aspose.cells/name/text/) { get; set; } | Obtiene el texto del nombre del objeto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Obtiene el rango si este nombre se refiere a un rango. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Obtiene el rango si este nombre se refiere a un rango |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Obtiene el rango si este nombre se refiere a un rango. Si la referencia de este nombre no es absoluta, el rango puede ser diferente para distintas celdas. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Obtiene todos los rangos referidos por este nombre. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Obtiene todos los rangos referidos por este nombre. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Obtiene todas las referencias referidas por este nombre. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Obtenga la referencia de este Name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Obtenga la referencia de este Name basada en la celda especificada. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Establezca la referencia de este Name. |
| override [ToString](../../aspose.cells/name/tostring/)() | Devuelve una cadena que representa el objeto Range actual. |

### Ejemplos

```csharp

[C#]

//Instanciando un objeto Workbook
Workbook workbook = new Workbook();
//Accediendo a la primera hoja de cálculo en el archivo Excel
Worksheet worksheet = workbook.Worksheets[0];
//Creando un rango con nombre
Range range = worksheet.Cells.CreateRange("B4", "G14");
//Estableciendo el nombre del rango nombrado
range.Name = "TestRange";
//Guardando el archivo de Excel modificado en el formato predeterminado (es decir, Excel 2000)
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Accessing the first worksheet in the Excel file
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Creating a named range
Dim range As Range = worksheet.Cells.CreateRange("B4", "G14")
'Setting the name of the named range
range.Name = "TestRange"
'Saving the modified Excel file in default (that is Excel 2000) format
workbook.Save("output.xls")
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


