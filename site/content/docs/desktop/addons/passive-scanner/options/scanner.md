---
# This page was generated from the add-on.
title: Passive Scanner
type: userguide
weight: 1
---

# Passive Scanner


This screen allows you to configure the passive scanner.

## Configuration Options

|                         Field                         |                                                                                                                                                                                 Details                                                                                                                                                                                  |  Default   |                                      Config File                                      |
|-------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------|---------------------------------------------------------------------------------------|
| Only scan messages in scope                           | Sets whether or not the passive scan should be performed only on messages that are in scope.                                                                                                                                                                                                                                                                             | Deselected | Key: `pscans.scanOnlyInScope` Values: `true` or `false`                               |
| Include traffic from the Fuzzer when passive scanning | Sets whether or not the passive scanning should be performed on messages generated by the Fuzzer.                                                                                                                                                                                                                                                                        | Deselected | Key: `pscans.scanFuzzerMessages` Values: `true` or `false`                            |
| Max alerts any rule can raise                         | Sets the maximum number of alerts a passive scan rule should raise. This may be slightly exceeded due to threading. This setting is typically only useful for automated scanning. Scan rules that exceed this value will be disabled and will need to be manually enabled if a new session is started.                                                                   | 0 (unset)  | Key: `pscans.maxAlertsPerRule` Values: `0`: unset or the maximum number of alerts     |
| Max body size in bytes to scan                        | Sets the maximum size request or response body size in bytes that the passive scanner will scan. This can be used if passive scan rules take too long scanning very large requests or responses. If set the number of ignored requests and responses are recorded in the stats using the keys `stats.pscan.reqBodyTooBig` and `stats.pscan.respBodyTooBig` respectively. | 0 (unset)  | Key: `pscans.maxBodySizeInBytes` Values: `0`: unset or the maximum body size in bytes |
| Clear Queue                                           | Empties the passive scan queue without passively scanning the messages. Currently running rules will run to completion but new rules will only be run when new messages are added to the queue.                                                                                                                                                                          |            |                                                                                       |

## See also

|   |                                                          |                                            |
|---|----------------------------------------------------------|--------------------------------------------|
|   | [Passive Scanner](/docs/desktop/addons/passive-scanner/) | the introduction to Passive Scanner add-on |