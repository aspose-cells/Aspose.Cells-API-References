##DigitalSignatureCollection
Provides a collection of digital signatures attached to a document.
## DigitalSignatureCollection class
Provides a collection of digital signatures attached to a document.
```javascript
class DigitalSignatureCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| The constructor of DigitalSignatureCollection. |
## Methods
| Method | Description |
| --- | --- |
| [add(DigitalSignature)](#add-digitalsignature-)| Add one signature to DigitalSignatureCollection. |
| [getEnumerator()](#getEnumerator--)| Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
The constructor of DigitalSignatureCollection.
```javascript
constructor();
```
### add(DigitalSignature) {#add-digitalsignature-}
Add one signature to DigitalSignatureCollection.
```javascript
add(digitalSignature: DigitalSignature) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| digitalSignature | [DigitalSignature](../digitalsignature/) | Digital signature in collection. |
### getEnumerator() {#getEnumerator--}
Get the enumerator for DigitalSignatureCollection, this enumerator allows iteration over the collection
```javascript
getEnumerator() : DigitalSignatureEnumerator;
```
**Returns**
The enumerator to iteration.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
