## Script: Get SQL Server Listening IPs and Ports

**Description**:
This script queries the dynamic management view `sys.dm_exec_connections` to return the list of local IP addresses and TCP ports used by SQL Server for active connections. Useful for:

- Verifying which IP/port SQL Server is actively using.
- Troubleshooting connectivity issues.
- Documenting server network configurations.

**Usage**:
Run the script on any SQL Server instance to return distinct active listening endpoints (IP and Port).

**Requirements**:
- Works on SQL Server 2005 and later.
- Requires `VIEW SERVER STATE` permission.
