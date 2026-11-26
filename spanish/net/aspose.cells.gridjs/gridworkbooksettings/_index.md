---
title: "Clase GridWorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridJs.GridWorkbookSettings. Representa la configuración del libro de trabajo"
type: docs
url: /es/net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Representa la configuración del libro de trabajo.

```csharp
public class GridWorkbookSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Obtiene/establece el autor del archivo. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Indica si se verifica el formato numérico personalizado al establecer Style.Custom, el valor predeterminado es false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Indica si se verifica la restricción del archivo excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, como mediante Cell.PutValue(string), si esta propiedad es true, obtendrás una Exception. Si la propiedad es false, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo excel, no deberías guardar el libro de trabajo como formato excel más adelante. De lo contrario, podría haber errores inesperados en el archivo excel generado. El valor predeterminado es false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Indica si se crea la cadena de fórmulas calculadas. El valor predeterminado es false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Obtiene o establece un valor que indica si el libro usa el sistema de fechas 1904. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Habilita macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro de trabajo. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Indica si se calcula completamente cada vez que se desencadena un cálculo. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Indica si se utiliza iteración para resolver referencias circulares. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Devuelve o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Indica si se recalculan todas las fórmulas al abrir el archivo. El valor predeterminado es true. |

### Ejemplos

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//realiza tu negocio

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### Ver también

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


