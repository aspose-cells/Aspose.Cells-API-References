##License
Provides methods to license the component.
## License class
Provides methods to license the component.
### Example
In this example, an attempt will be made to find a license file named Aspose.Cells.lic in the input folder that contains the component, in the folder that contains the calling assembly,in the folder of the entry assembly and then in the embedded resources of the calling assembly.
```javascript
const { License } = require("aspose.cells.node");
var license = new License();
license.setLicense("input/Aspose.Cells.lic");
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of this class. |
## Methods
| Method | Description |
| --- | --- |
| [setLicense(string)](#setLicense-string-)| Licenses the component. |
| [setLicense(Uint8Array)](#setLicense-uint8array-)| Licenses the component. |
### constructor() {#constructor--}
Initializes a new instance of this class.
```javascript
constructor();
```
### setLicense(string) {#setLicense-string-}
Licenses the component.
```javascript
setLicense(licenseName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| licenseName | string | The license file path. |
### setLicense(Uint8Array) {setLicense-uint8array-}
Licenses the component.
```javascript
setLicense(stream: Uint8Array): void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | A stream that contains the license. |
