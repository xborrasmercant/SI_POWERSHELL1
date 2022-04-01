# Ejercicio de clase 3. Primitive Datatype tasks
## Xavier Borrás Mercant


### 1. Use “Get-Help” to find out more information about 5 cmdlets.
- `Get-Help Get-Process`
- `Get-Help Clear-History`
- `Get-Help Where-Object`
- `Get-Help Clear-Content`
- `Get-Help ConvertTo-XML`

### 2. Use “Get-Help” with the “–Example” parameter for the 5 cmdlets you discovered more about in task 1.
- `Get-Help Get-Process -Examples`
- `Get-Help Clear-History -Examples`
- `Get-Help Where-Object -Examples`
- `Get-Help Clear-Content -Examples`
- `Get-Help ConvertTo-XML -Examples`

### 3. Create a new text file named “TestFile.txt” under C:\Maximo\PowerShell\Workshop1\%USERNAME%.
- `New-Item -Path C:\Maximo\PowerShell\Workshop1 -Name %USERNAME% -ItemType Directory`
- `New-Item -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\ -Name TestFile.txt -ItemType File`

### 4. Populate the text file you created in task 3 with all three datatypes we’ve covered: “Boolean”, “String” and “Int”.
- `Add-Content -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\Testfile.txt -Value True`
- `Add-Content -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\Testfile.txt -Value "Hello"`
- `Add-Content -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\Testfile.txt -Value 42`

### 5. Read from the text file and use “Get-Member” to find the datatype returned.
- `Get-Content -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\Testfile.txt | Get-Member`

### 6. Overwrite all data within the text file that you created in task 3.
- `Set-Content -Path C:\Maximo\PowerShell\Workshop1\%USERNAME%\Testfile.txt -Value "Boooooo"`

### 7. Format the data returned by a cmdlet into a list.
- `Get-Service | Format-List`

### 8. Pipe “Get-Command” into “Out-GridView”.
- `Get-Command | Out-GridView`

### 9. Pipe the 5 cmdlets you discovered in task 1 into “Out-GridView”
- `Get-Process | Out-GridView`
- `Clear-History | Out-GridView`
- `Where-Object | Out-GridView`
- `Clear-Content | Out-GridView`
- `ConvertTo-XML | Out-GridView`

### 10. Find the official PowerShell documentation library from Microsoft

- https://docs.microsoft.com/en-us/powershell/
