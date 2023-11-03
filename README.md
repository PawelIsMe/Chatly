# Chatly
Początkowy pomysł programu chatly był taki, żeby użytkownicy wchodząc na strone ujrzeli czat i mogli na nim bez problemowo pisać, będąc przy tym anonimowym i bez żadnej historii czatu (gdy użytkownik odświeży strone to historia czatu się zresetuje). Jednak, gdy doszedłem do takiego poziomu chatly jak powyżej, to pomyślałem sobie, czemu by nie dodać tu interfejsu logowania i rejestracji oraz historii czatu. Od tego właśnie wszystko się zaczęło. Gdy zacząłem rozwijać swój pomysł, zacząłem prace od frontendu. A więc najpierw zaprojektowałem swój projekt w figmie, potem przepisałem go na html-a i css-a (oczywiście troche się różni niż w figmie, ze względu na to, że zawsze coś zmieniam gdy przepisuje na html-a), a następnie zrobiłem do tego cały backend. Interfejs rejestracji polega na tym, że program zapisuje dane użytkownika (po ich podaniu) do pliku accounts.json, a potem gdy użytkownik chce się zalogować na strone to musi podać nazwe użytkownika i hasło, jakie podał przy tworzeniu konta. Do tego działa również auto login, który pobiera adres IP danego użytkownika i gdy wchodzi na strone localhost:5000/ to server go autoryzuje i automatycznie przekierowuje na stronę z czatem. Oczywiście użytkownik może również się wylogować naciskając przycisk umieszczony w lewym dolnym rogu 'Log out', wtedy opcja zamieszczona w pliku accounts.json, 'islogged' zmienia się z 1 na 0. Oprócz tego backend również dotyczy wspomnianej historii czatu. Działa to w ten sposób, że gdy server otrzyma wiadomość, którą wysyła użytkownik to ją zapisuje w pliku conversation.txt w formie \<div\> lub \<p\>, w zależności od tego który użytkownik wysłał wiadomość. Nie ukrywam, że działa to w podobny spoób jak na discordzie, ponieważ właśnie tym m.in. się posiłkowałem. Do tego musiałem również użyć biblioteki regex, żeby dowiedzieć się który użytkownik wysłał poprzednią wiadomość. Program powinien być kompatybilny z windowsem i linuxem. A i jeszcze należałoby nadmienić, że program działa w sieci lokalnej (na zewnątrz nie testowałem).

# Logowanie
![image](https://github.com/PawelIsMe/Chatly/assets/107412394/55f4d74e-0c64-4392-8f1e-cbca5e00c3eb)


# Rejestracja
![image](https://github.com/PawelIsMe/Chatly/assets/107412394/33df60e6-1208-40f9-adbe-bbaee49d14f9)


# Czat z animacją (animacja napisana w js)
![image](https://github.com/PawelIsMe/Chatly/assets/107412394/d87f372f-dc67-45cb-981f-0a098b5899d8)


# Czat
![image](https://github.com/PawelIsMe/Chatly/assets/107412394/d38437e3-a598-4715-b3fe-b4c7db07593a)
