# PS-HostPortChecker
Powershell: Check port status for target hosts.

.EXAMPLE
    .\Network-CheckPortsByArray.ps1 -hosts 10.0.10.1,ts-core-rt01 -ports 22,80,443
    
    .\Network-CheckPortsByArray.ps1 -hosts 10.0.10.1,ts-core-rt01 -ports 22,80,443 -exportCSV $true -outfile 'C:\temp\Get-HostsPortStatus.csv'
    
.INPUTS
   Hosts - IPaddress or hostname (separated by ',').
   Ports - List of ports to check (separated by ','). 
   
.OUTPUTS
   Terminal output. OPTIONAL: CSV export.
