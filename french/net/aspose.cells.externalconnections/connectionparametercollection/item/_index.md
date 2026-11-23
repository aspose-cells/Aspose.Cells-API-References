---
title: "ConnectionParameterCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameterCollection. Obtient l'élément ConnectionParameter à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Obtient l'élément [`ConnectionParameter`](../../connectionparameter/) à l'index spécifié.

```csharp
public ConnectionParameter this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenir la première connexion externe
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Obtenir la collection de paramètres
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Vérifier s'il existe des paramètres avant d'accéder
                if (parameters.Count > 0)
                {
                    // Démontrer la lecture de la propriété Item
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Obtient l'élément [`ConnectionParameter`](../../connectionparameter/) avec le nom spécifié.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Paramètre | Description |
| --- | --- |
| connParamName | nom du paramètre de connexion |

### Valeur de retour

L'élément avec le nom spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Obtenir la première connexion externe
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Obtenir la collection de paramètres
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Vérifier s'il existe des paramètres existants pour démontrer la propriété Item
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Obtenir le nom du premier paramètre à utiliser pour la démonstration
                string firstParamName = parameters[0].Name;
                
                // Démontrer la lecture de la propriété Item par nom
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


