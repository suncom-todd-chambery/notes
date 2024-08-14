---
id: rcxz6nuilmnqbzaiuqqj3tf
title: wo 4519692337 - VPN2 LAN to LAN - Change VPN Tunnels
desc: ''
updated: 1723651551396
created: 1723557442526
---


This is the order that carried on sending after the `com.harris.hten.bits.common.exception.order.CannotProcessOrderLvStateException` exception.

I rejected the order back to Engineering "awaiting `updateOrderPending`"

The order was then modified by Zachary Adler, but his changes are not showing up in the order Revision as sent to the customer:

"Objective was to revise the order removing LAN source `192.0.0.254/32` and replace with `10.14.184.8/29`."

Asked Nelson where work order revision changes live, `sc_dtl_id`

`select oasis_detail.from_network_ref(4519692551) from dual;`
`sc_dtl_id` -> 

Changes were never recorded.

Nelson reccomended rejecting retrying 

##### Nelson Blocker  11:01 AM
> The revision data was correct, it just won't show in the task list. Create the revision one more time, and then look at the corresponding `SERVICE_CONFIGURATION_REVISION` record, `SCR_DATA` field. I'd like to look at the revision again after you create it.


