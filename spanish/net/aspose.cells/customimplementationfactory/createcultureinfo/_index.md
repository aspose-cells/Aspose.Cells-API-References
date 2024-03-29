---
title: CreateCultureInfo
second_title: Referencia de API de Aspose.Cells para .NET
description: Crear un CultureInfo por id dado.
type: docs
weight: 20
url: /es/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Crear un CultureInfo por id dado.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| lcid | Int32 |  |

### Valor_devuelto

La instancia de CultureInfo.

### Observaciones

Esta implementación es útil para situaciones: 1. Es posible que el entorno del usuario no admita algunas culturas y crear el CultureInfo requerido con el identificador dado puede causar una excepción. Para evitar la excepción, el usuario puede anular este método para proporcionar una instancia de CultureInfo válida para el uno no compatible. 2. El usuario puede querer especificar algunas propiedades personalizadas para algunas culturas para obtener el resultado esperado para el formato. Para este propósito, el usuario puede anular este método para proporcionar a la instancia de CultureInfo las propiedades especificadas por el usuario. Tenga en cuenta la propiedad UseUserOverride del La instancia de CultureInfo devuelta puede influir en el resultado formateado. Si es falso, algunas propiedades de la instancia de CultureInfo devuelta pueden ser anuladas por nuestro motor de formato integrado de acuerdo con los requisitos de formato de diferentes escenarios. Si es verdadero, no lo haremos cambie cualquier propiedad y utilícelo para formatear valores directamente. Entonces, si el usuario tiene spe propiedades personalizadas especificadas para la instancia de CultureInfo devuelta, asegúrese de que UseUserOverride sea verdadero.

### Ver también

* class [CustomImplementationFactory](../../customimplementationfactory)
* espacio de nombres [Aspose.Cells](../../customimplementationfactory)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
