# Скопируйте clinic-offline.zip на целевую систему 

# Распакуйте его:
# unzip clinic-offline.zip -d clinic
# cd clinic

# Установите зависимости
# for file in *.tgz; do
#   if [[ "$file" != clinic* ]]; then
#     npm install -g "./$file"
#   fi
# done

# Установите clinic
# npm install -g ./clinic-*.tgz
