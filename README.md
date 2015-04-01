[![Build Status](https://secure.travis-ci.org/gilt/gfc-timeuuid.png)](http://travis-ci.org/gilt/gfc-timeuuid)

# Gfc TimeUuid

An timeuuid library in Scala base on http://www.ietf.org/rfc/rfc4122.txt which generates version 1 UUIDs.

## Example Usage
Generates a new unique time based UUID

    val uuid = TimeUuid()

Convert time UUID to unix timestamp

    import com.gilt.timeuuid._

    val uuid = TimeUuid()
    val timestamp = uuid.toLong

Convert time UUID to unix date

    import com.gilt.timeuuid._

    val uuid = TimeUuid()
    val date = uuid.toDate

Convert arrays of 16 bytes to UUID:
    val bytes = new Array[Byte](16)
    val uuid = bytes.toUUID

## License
Copyright 2014 Gilt Groupe, Inc.

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
