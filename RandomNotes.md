#Random Notes - 4 days into the project

"Real" IDM at Idp - ie. no persistence of actual data in Stinus - except for hashes of sent/received.

Stinus can run at Idp or at Fed Operator.

Repository of connectors - also for use outside Stinus?

Should Stinus keep hash of received data - schemachanges at Sp connector might invalidate?

Stinus is one connection from the Idp - schema- and feedwise
Stinus is Idp push only - but can pull from Idp if needed. Ie. no pull from Sp.

But multiple Idp feeds to one Sp should be supported - poor mans VO eg. for xtra attributes not in main directory

Stinus can feed a pseudo Sp - with storage - for aggreation which can then be feed into Stinus again.

Writing is expensive - Reading is cheap

Changes are rare

Stinus supports partial feeds and event driven feeds

Standard connectors for common schemas eg. AD (and ldap?)

SyncModes
  * Force - just write record
  * Hard - read, compare and write on change
  * Soft - cmp with hash and write on change

UpdateModes
  * Partial, Full
  * Ldap: replace specific values?

Common Cannonical Schema - ???
Support for specific schemas (pass-thru) btw. Idp and Sp.

Issues:

  * Google can do batch reads - but recs come back in random order

Random ideas:

  * Obfuscation a la UnboundID Sync Server data ie. read prod data and convert to ubfuscated test data
