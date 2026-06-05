# Lab14

# Uruchomienie środowiska
za pomoca polecenia docker compose up -d beda w folderze urcuhmammy środowisko
<img width="979" height="216" alt="image" src="https://github.com/user-attachments/assets/324c0449-c31a-40a5-b1f8-8d1f8f58b822" />
Sprawdzamy status za pomoca docker compose ps
<img width="981" height="169" alt="image" src="https://github.com/user-attachments/assets/5f38521b-106f-47d0-81dd-fb98fa8898e7" />


# Weryfikacja
Sprawdzamy dziąłanie strony na adresie http://localhost:4001/
<img width="1253" height="682" alt="image" src="https://github.com/user-attachments/assets/6f4244f0-307f-43fa-b29f-79e04f217b26" />

# Baza danych
Wchodzimy na http://localhost:6001/ i logujemy sie do używając danych zadeklarownych user: root passsowrd: rootpassword gdzie tworze baze danych lab14. Phpmyadmin jest przypisany do frontendu oraz do backundu. Sieć backend jest niezbędna do komunkacji z kontenerm mysql, pozwala na nazwy hosta . Sieć fronrend jest konieczna do interfejsu webowego dla użytkownika i umożliwia bezpieczną separację ruchu zewnętrznego od wewnętrznej sieci bazy danych
<img width="1365" height="447" alt="image" src="https://github.com/user-attachments/assets/73beacfd-4d82-4958-8183-7a0feaad0064" />

# Dotakowe zadani
Czyszczenie wolumenów poleceniem docker compose down -v
<img width="979" height="160" alt="image" src="https://github.com/user-attachments/assets/43ff66a5-7e2e-41a4-9348-147dbde7a525" />

Uruchomienie zaktualnowanego środwiska docker compose up -d
<img width="984" height="175" alt="image" src="https://github.com/user-attachments/assets/774973a5-cb62-492c-bdd1-5e692a723da6" />

Polecnie docker container inspect mysql_server | Select-String -Pattern '"Destination": "/run/secrets/db_root_password"' -Context 0,5 spowodowało poprawne wysłanie piliku z danymi wrażliwymi do struktury kontera i jest w trybie tylko do odczytu "RW" : false
<img width="990" height="157" alt="image" src="https://github.com/user-attachments/assets/a9e83185-362d-4291-b7d4-e116067e9ff8" />

Sprawdzamy dziąłanie strony na adresie http://localhost:4001/
<img width="1366" height="681" alt="image" src="https://github.com/user-attachments/assets/58906357-baec-429c-b7dd-f6ef68e83b23" />

Wchodzimy na http://localhost:6001/ i logujemy sie do używając danych zadeklarownych user: root passsowrd: TajneHasloBazy123 haslo w pliku db_root-password.txt
<img width="1366" height="423" alt="image" src="https://github.com/user-attachments/assets/5730d0a9-c77b-4c61-8cd1-71e63b96c8ac" />


<img width="1363" height="342" alt="image" src="https://github.com/user-attachments/assets/aeb443b3-cef8-4a3e-88c7-6c1bcf2d83a1" />
