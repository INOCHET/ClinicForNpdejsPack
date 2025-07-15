Скопируйте clinic-offline.zip на целевую систему 

# Распакуйте его:
Expand-Archive -Path clinic-offline.zip -DestinationPath clinic-offline
cd clinic-offline

# Установите зависимости
Get-ChildItem *.tgz | Where-Object { $_.Name -ne "clinic-*.tgz" } | ForEach-Object {
    npm install -g $_.Name
}

# Установите clinic
npm install -g clinic-*.tgz
