---
title: "Aspose.Cells.GridJs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "L'espace de noms Aspose.Cells.GridJs encapsule toutes les classes de GridJs offrant des API simples pour visualiser ou modifier des fichiers de feuilles de calcul via des opérations JSON."
type: docs
url: /fr/net/aspose.cells.gridjs/
---
L'espace de noms **Aspose.Cells.GridJs** encapsule toutes les classes de GridJs, offrant des API simples pour visualiser ou modifier des fichiers de feuilles de calcul via des opérations JSON.

## Classes

| Classe | Description |
| --- | --- |
| [Config](./config/) | Représente tous les paramètres statiques pour GridJs. |
| [DefaultGridJsJsonCache](./defaultgridjsjsoncache/) | Implémentation par défaut du cache JSON (mémoire L1 + disque L2) |
| [GridAbstractCalculationEngine](./gridabstractcalculationengine/) | Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells. |
| [GridCacheForStream](./gridcacheforstream/) | Cette classe contient les opérations de cache pour GridJs. L'utilisateur doit implémenter sa propre logique métier pour le stockage basée sur celle-ci.. |
| [GridCalculationData](./gridcalculationdata/) | Représente les données requises lors du calcul d'une fonction, telles que le nom de la fonction, les paramètres, ...etc. |
| [GridCellException](./gridcellexception/) | L'exception qui est levée lorsqu'une erreur spécifiée de GridJs se produit. |
| [GridInterruptMonitor](./gridinterruptmonitor/) | Représente tous les opérateurs concernant l'interruption du calcul. |
| [GridJsControllerBase](./gridjscontrollerbase/) |  |
| [GridJsLogger](./gridjslogger/) | Fournit un système de journalisation léger pour le serveur GridJs. Prend en charge la sortie console et fichier avec des niveaux de journalisation configurables. Le niveau par défaut est Aucun. Dans une version DEBUG, le niveau par défaut est Debug (affiche tous les messages). Prend en charge la rotation des fichiers journaux par jour/semaine/mois. |
| [GridJsOptions](./gridjsoptions/) | Représente toutes les options de chargement pour GridJs |
| [GridJsPermissionException](./gridjspermissionexception/) | représente une exception d'autorisation en mode collaboration. Disponible uniquement dans la version Java pour le moment, sera disponible dans les versions .net/python à l'avenir. |
| [GridJsService](./gridjsservice/) | Fournit les API d'opération de base utilisées dans les actions du contrôleur. |
| [GridJsWorkbook](./gridjsworkbook/) | Représente la classe principale d'entrée pour GridJs |
| [GridReferredArea](./gridreferredarea/) | Représente une zone référencée par la formule. |
| [GridUpdateMonitor](./gridupdatemonitor/) | Moniteur pour l'utilisateur afin de suivre le changement de l'opération de mise à jour. |
| [GridWorkbookSettings](./gridworkbooksettings/) | Représente les paramètres du classeur. |
| [JsonCacheOptions](./jsoncacheoptions/) | Options de configuration pour la mise en cache JSON dans GridJs. Contrôle le comportement du cache mémoire (L1) et disque (L2). |
| [OprMessageService](./oprmessageservice/) | Cette classe fournit toutes les opérations de synchronisation des messages en mode collaboratif. |
## Interfaces

| Interface | Description |
| --- | --- |
| [CoWorkUserProvider](./coworkuserprovider/) | Représente l'interface du fournisseur d'utilisateurs en mode collaboration. Disponible uniquement dans la version Java pour le moment, sera disponible dans les versions .net/python à l'avenir. L'application cliente peut implémenter cette interface pour fournir les informations utilisateur. |
| [IGridJsJsonCache](./igridjsjsoncache/) | Interface de cache JSON - les clients implémentent des stratégies de stockage et d'invalidation spécifiques |
| [IGridJsService](./igridjsservice/) | Représente l'interface des API d'opération de base utilisées dans les actions du contrôleur. |
| [ITextTranslator](./itexttranslator/) | Représente l'interface de traduction |
## Énumération

| Énumération | Description |
| --- | --- |
| [CoWorkOperationType](./coworkoperationtype/) | Représente le type d'opération d'action en mode collaboration. Disponible uniquement dans la version Java pour le moment, sera disponible dans les versions .net/python à l'avenir. |
| [CoWorkUserPermission](./coworkuserpermission/) | représente l'autorisation de l'utilisateur en mode collaboration. Disponible uniquement dans la version Java pour le moment, sera disponible dans les versions .net/python à l'avenir. |
| [GridExceptionType](./gridexceptiontype/) | Représente le code d'exception personnalisé pour GridJs. |
| [GridJsLogLevel](./gridjsloglevel/) | Spécifie le niveau de journalisation pour le logging de GridJs. |
| [GridJsLogRolling](./gridjslogrolling/) | Spécifie la stratégie de rotation des fichiers journaux. |
| [GridLoadFormat](./gridloadformat/) | Représente le format de fichier de chargement. |


