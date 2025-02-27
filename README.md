# Purview-Power-Shell
Microsoft Purview data security solutions help you manage and monitor your data and protect information

PowerShell command 

# Install the Az module if you haven't already
Install-Module -Name Az -AllowClobber -Force

# Import the Az module
Import-Module -Name Az

# Connect to your M365 admin account
Connect-IPPSSession

# List all Purview label in your org
Get-Label

# List all Purview label policy in your org
Get-LabelPolicy

# To select and display only the name property of each service object Purview label policy in your org
Get-LabelPolicy | Select-Object -ExpandProperty Name
