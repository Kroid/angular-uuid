angular-uuid
============

angular.module('your-app', ['kroid-uuid'])



Generate a random uuid.
Based on Math.uuid.js (v1.4) ( http://www.broofa.com mailto:robert@broofa.com 2010 Robert Kieffer )

USAGE: uuid(length, radix)
 length - the desired number of characters
 radix  - the number of allowable values for each character.

EXAMPLES:
  No arguments  - returns RFC4122, version 4 ID
   >>> uuid()
  "92329D39-6F5C-4520-ABFC-AAB64544E172"

  One argument - returns ID of the specified length
  >>> uuid(15)     // 15 character ID (default base=62)
  "VcydxgltxrVZSTV"

  // Two arguments - returns ID of the specified length, and radix. (Radix must be <= 62)
  >>> uuid(8, 2)  // 8 character ID (base=2)
  "01001010"
  >>> uuid(8, 10) // 8 character ID (base=10)
  "47473046"
  >>> uuid(8, 16) // 8 character ID (base=16)
  "098F4D35"
