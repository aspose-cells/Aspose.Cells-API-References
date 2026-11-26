---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomImplementationFactory. Crea un CultureInfo con el id proporcionado"
type: docs
url: /es/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Crea un CultureInfo a partir del id proporcionado.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| lcid | Int32 |  |

### Valor de retorno

La instancia de CultureInfo.

### Observaciones

Esta implementación es útil en las siguientes situaciones: 1. Algunas culturas pueden no ser compatibles con el entorno del usuario y crear el CultureInfo requerido con el identificador dado puede generar una excepción. Para evitar la excepción, el usuario puede sobrescribir este método para proporcionar una instancia válida de CultureInfo para la que no está soportada. 2. El usuario puede querer especificar algunas propiedades personalizadas para ciertas culturas para obtener el resultado esperado al formatear. Con este fin, el usuario puede sobrescribir este método para proporcionar la instancia de CultureInfo con las propiedades especificadas por el usuario. Tenga en cuenta que la propiedad UseUserOverride de la instancia de CultureInfo devuelta puede influir en el resultado formateado. Si es false, algunas propiedades de la instancia de CultureInfo devuelta pueden ser sobrescritas por nuestro motor de formato incorporado según los requisitos de formato de diferentes escenarios. Si es true, no cambiaremos ninguna propiedad y la utilizaremos para formatear valores directamente. Por lo tanto, si el usuario ha especificado propiedades personalizadas para la instancia de CultureInfo devuelta, asegúrese de que su UseUserOverride sea true.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Crea una instancia de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Llame a CreateCultureInfo con un LCID válido (1033 para Inglés - Estados Unidos)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Muestra los resultados
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Demuestre la configuración de la fábrica en CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


