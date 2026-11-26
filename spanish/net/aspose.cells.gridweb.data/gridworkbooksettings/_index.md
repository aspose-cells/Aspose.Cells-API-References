---
title: "Clase GridWorkbookSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridWorkbookSettings. Representa la configuración del libro de trabajo"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

Representa la configuración del libro de trabajo.

```csharp
public class GridWorkbookSettings : ISerializable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author/) { get; set; } | Obtiene y establece el autor del archivo. |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Obtiene o establece si se verifica el formato de número personalizado al establecer Style.Custom. |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain/) { get; set; } | Obtiene o establece si se crea una cadena de fórmulas calculadas. El valor predeterminado es false. |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904/) { get; set; } | Obtiene o establece el valor que indica si el libro de trabajo usa el sistema de fechas 1904. |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros/) { get; set; } | Obtiene o establece si se habilitan las macros; ahora solo funciona al copiar una hoja de cálculo a otra hoja dentro de un libro de trabajo. |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate/) { get; set; } | Obtiene o establece si se calcula completamente cada vez que se desencadena un cálculo. |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration/) { get; set; } | Obtiene o establece si se utiliza iteración para resolver referencias circulares. |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration/) { get; set; } | Obtiene o establece el número máximo de iteraciones para resolver una referencia circular, el valor predeterminado es 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True si los cálculos en este libro de trabajo se realizarán usando solo la precisión de los números tal como se muestran |
| [PreservePaddingSpaces](../../aspose.cells.gridweb.data/gridworkbooksettings/preservepaddingspaces/) { get; set; } | Indica si se conservan los espacios y saltos de línea que se insertan entre los tokens de la fórmula al obtener y establecer fórmulas. El valor predeterminado es false. |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen/) { get; set; } | Obtiene o establece si se recalculan todas las fórmulas al abrir el archivo. |

### Ejemplos

```csharp
[C#]

 
GridWeb gridweb = new GridWeb();
GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//realiza tu negocio

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb.Settings=gsettings;
 
'do your business
```

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


