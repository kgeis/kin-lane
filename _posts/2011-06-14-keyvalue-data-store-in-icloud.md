---
layout: post
title: Key-Value Data Store in iCloud
url: http://apievangelist.com/2011/06/14/key-value-data-store-in-icloud/
source: http://apievangelist.com/2011/06/14/key-value-data-store-in-icloud/
domain: apievangelist.com
image: http://kinlane-productions.s3.amazonaws.com/apple/icloud-stainless-3-devices-key-value.png
---
{% include JB/setup %}<p>Apples new iCloud platform includes a new key-value data store, along side its document storage.An application can use the key-value data store to put small amounts of data in the cloud, and share with other instances of the same application running on other computers and IOS devices.The key-value data store is meant to save simple data types (numbers, strings, dates, and arrays) persistently and retrieve later.The amount of available space in a single key-value store is limited to 64 KB and the data for a single key cannot exceed 4 KB.This size allows the storage of small details from an application, but should not be used to store user documents or other large data objects, this should be done with iCloud document storage.</p>

