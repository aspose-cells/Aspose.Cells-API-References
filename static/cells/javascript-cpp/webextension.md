##WebExtension
Represents an Office Addin instance.
## WebExtension class
Represents an Office Add-in instance.
```javascript
class WebExtension;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [id](#id--)| string | Gets and sets the uniquely identifies the Office Add-in instance in the current document. |
| [isFrozen](#isFrozen--)| boolean | Indicates whether the user can interact with the Office Add-in or not. |
| [reference](#reference--)| WebExtensionReference | Readonly. Get the primary reference to an Office Add-in. |
| [alterReferences](#alterReferences--)| WebExtensionReferenceCollection | Readonly. Gets a list of alter references. |
| [properties](#properties--)| WebExtensionPropertyCollection | Readonly. Gets all properties of web extension. |
| [bindings](#bindings--)| WebExtensionBindingCollection | Readonly. Gets all bindings relationship between an Office Add-in and the data in the document. |
### id {#id--}
Gets and sets the uniquely identifies the Office Add-in instance in the current document.
```javascript
id : string;
```
### isFrozen {#isFrozen--}
Indicates whether the user can interact with the Office Add-in or not.
```javascript
isFrozen : boolean;
```
### reference {#reference--}
Readonly. Get the primary reference to an Office Add-in.
```javascript
reference : WebExtensionReference;
```
### alterReferences {#alterReferences--}
Readonly. Gets a list of alter references.
```javascript
alterReferences : WebExtensionReferenceCollection;
```
### properties {#properties--}
Readonly. Gets all properties of web extension.
```javascript
properties : WebExtensionPropertyCollection;
```
### bindings {#bindings--}
Readonly. Gets all bindings relationship between an Office Add-in and the data in the document.
```javascript
bindings : WebExtensionBindingCollection;
```
