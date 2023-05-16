---
title: "HelloWorld"
date: 2023-05-16T01:20:29-07:00
author: Joel Reed
---

## Hello World

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

```PowerShell
while ($true) {
    Clear-Host
    1..250 | ForEach-Object {
        Write-Progress -Activity 'Attempting to connect' -Status 'decrypting...' -PercentComplete $(($wp / $(250)) * 100) -Id 1
        $line = [string]::Empty
        while ($line.Length -lt 100) {
            $n = Get-Random -Maximum 126 -Minimum 33
            $line += "$(' ' * ($n%3))$([char][byte]$n)$(' ' * ($n%2))"
        }
        Write-Host $line -ForegroundColor Green
        Start-Sleep -Milliseconds 25
    }
    Write-Progress -Activity 'Done' -Id 1 -Completed
    Clear-Host
    '32', '32', '95', '95', '32', '95', '32', '32', '32', '32', '32', '95', '32', '13', '10', '32', '47',
    '32', '95', '124', '32', '124', '32', '32', '32', '40', '95', '41', '13', '10', '124', '32', '124',
    '95', '124', '32', '124', '95', '95', '32', '32', '95', '32', '13', '10', '124', '32', '32', '95',
    '124', '32', '39', '95', '32', '92', '124', '32', '124', '13', '10', '124', '32', '124', '32', '124',
    '32', '124', '95', '41', '32', '124', '32', '124', '13', '10', '124', '95', '124', '32', '124', '95',
    '46', '95', '95', '47', '124', '95', '124' | ForEach-Object { 
        Write-Host "$([char][byte]$_)" -NoNewline -ForegroundColor Green
    }
    Write-Host "`n`nEstablishing session" -ForegroundColor Cyan -NoNewline
    1..10 | ForEach-Object {
        Write-Host '.' -NoNewline -ForegroundColor Cyan
        Start-Sleep -Milliseconds 250
    }
    1..3 | ForEach-Object {
        Write-Host "`n`npasscode > " -NoNewline
        $n = Get-Random -Maximum 24 -Minimum 8
        for ($i = 0; $i -lt $n; $i++) {
            Write-Host '*' -NoNewline -ForegroundColor Gray
            Start-Sleep -Milliseconds 250
        }
        Write-Host "`naccess denied!" -ForegroundColor Red
    }
    Write-Host "`ndisconnecting and reporting" -ForegroundColor Red -NoNewline
    1..10 | ForEach-Object {
        Write-Host '.' -NoNewline -ForegroundColor Red
        Start-Sleep -Milliseconds 250
    }
}
```

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
