## Designing a Custom Identity Pallet

In this example we are trying to design an identity pallet, where: <br />
Users could generate a new identity <br />
Add/remove attributes to that identity <br />
Delete the identity <br />

## Storage Items <br />
Identity map: Identity => AccountId <br />
Attribute map: (Identity, Attribute_Key) => Attribute_Value <br />

## Events <br />
IdentityCreated(Identity, AccountId) <br />
AttributeAdded(Identity, Attribute_Key, Attribute_Value) <br />
AttributeRemoved(Identity, Attribute_Key), <br />

## Errors <br />
IdentityAlreadyClaimed <br />
IdentityNotFound <br />
NotAuthorized <br />
AttributeNotFound <br />

##Function Calls <br />
create_identity( Identity ) <br />
add_attribute( Identity, Attribute_Key, Attribute_Value ) <br />
remove_attribute( Identity, Attribute_Key ) <br />


