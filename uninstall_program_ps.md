# uninstall program

## step 1 : find proper program name

```
Get-WmiObject -Class Win32_Product | Select-Object -Property Name
```

## step 2 : save the program into a variable

for example, if the program is called "Free Tools"

```
$MyApp = Get-WmiObject -Class Win32_Product | Where-Object{$_.Name -eq "Free Tools"}
```

## step 3 : uninstall the program
```
$MyApp.Uninstall()
```
