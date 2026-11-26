---
title: "GridLoadOptions.CheckExcelRestriction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "GridLoadOptions propiedad. Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena más largo que 32 K. Cuando ingresas un valor más largo que 32 K, por ejemplo mediante Cell.PutValuestring, si esta propiedad es verdadera obtendrás una excepción. Si esta propiedad es falsa aceptaremos tu valor de cadena como el valor de la celda, de modo que luego puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un tipo de valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario, puede haber errores inesperados en el archivo Excel generado."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/
---
## GridLoadOptions.CheckExcelRestriction property

Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor superior a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si esta propiedad es falsa, aceptaremos la cadena introducida como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro posteriormente en formato Excel. De lo contrario, podría producirse un error inesperado en el archivo Excel generado.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Ver también

* class [GridLoadOptions](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


