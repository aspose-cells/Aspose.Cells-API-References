---
title: "GridWorkbookSettings.CheckExcelRestriction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridWorkbookSettings. Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32K. Cuando introduces un valor más largo que 32K, como mediante Cell.PutValuestring, si esta propiedad es true obtendrás una excepción. Si la propiedad es false aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro de trabajo en formato Excel más adelante. De lo contrario, pueden producirse errores inesperados en el archivo Excel generado. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/
---
## GridWorkbookSettings.CheckExcelRestriction property

Indica si se verifica la restricción del archivo excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, excel no permite ingresar un valor de cadena mayor a 32 K. Cuando ingresas un valor mayor a 32 K, como mediante Cell.PutValue(string), si esta propiedad es true, obtendrás una Exception. Si la propiedad es false, aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo excel, no deberías guardar el libro de trabajo como formato excel más adelante. De lo contrario, podría haber errores inesperados en el archivo excel generado. El valor predeterminado es false.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Ver también

* class [GridWorkbookSettings](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


