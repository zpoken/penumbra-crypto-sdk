## 🚴 Usage

### Install package
```
npm i penumbra-web-assembly@v0.1.7
```
### Example of usage
```
import {decrypt_note} from "penumbra-web-assembly";

let decryptedNote 
= decrypt_note("<penumbrafullviewingkey>", "<encrypted_note hex>", "<ephemeral_key hex>");

console.log(decryptedNote);
```
#### If the FVK was able to decrypt the note successfully, the function will return an object with the following set of fields
```
diversifier: "0c20467296f5e78d622eaf"
note_blinding: "0c1e49ba245bb661419785d4cd599c212e43cc1d800dc62863fd66ef734a6511"
transmission_key: "046d8263d8da27c3265672080e98dce936d84954428bd1905686fb8a860c890b"
value:
  amount: 998000000
  asset_id: "passet1984fctenw8m2fpl8a9wzguzp7j34d7vravryuhft808nyt9fdggqxmanqm"
```
