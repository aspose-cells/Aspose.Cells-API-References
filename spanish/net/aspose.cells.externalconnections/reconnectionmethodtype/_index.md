---
title: "Enum ReConnectionMethodType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType enum. Especifica lo que la aplicación de hoja de cálculo debe hacer cuando una conexión falla"
type: docs
url: /es/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Especifica lo que la aplicación de hoja de cálculo debe hacer cuando falla una conexión.

```csharp
public enum ReConnectionMethodType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Required | `1` | Al actualizar, use la información de conexión existente y, si resulta ser inválida, obtenga información de conexión actualizada, si está disponible en el archivo de conexión externa. |
| Always | `2` | En cada actualización, obtenga información de conexión actualizada del archivo de conexión externa, si está disponible, y utilícela en lugar de la información de conexión existente. En este caso, la actualización de datos fallará si el archivo de conexión externa no está disponible. |
| Never | `3` | Nunca obtenga información de conexión actualizada del archivo de conexión externa, incluso si está disponible y aunque la información de conexión existente sea inválida |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Demostrar la creación y uso de valores del enum ReConnectionMethodType
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Mostrar uso en una sentencia switch
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


