# Bezpieczeństwo: hasła i klucze w repozytorium

Repozytorium jest publiczne, więc każdy plik może przeczytać i pobrać (sklonować) dowolna osoba na świecie, także automatyczne boty, które przeszukują GitHub w poszukiwaniu haseł i kluczy dostępu. Klucz do płatnej chmury znaleziony w ten sposób może w kilka minut posłużyć do uruchomienia drogich zasobów na koszt właściciela.
Samo usunięcie pliku nie wystarcza, bo Git przechowuje całą historię zmian: usunięcie to tylko kolejne zatwierdzenie, a poprzednie wersje pliku, razem z hasłem, nadal da się obejrzeć w zakładce Commits (tak jak w zadaniu 11). Ponadto ktoś mógł już wcześniej sklonować repozytorium i mieć własną kopię.
Dlatego wyciekłe hasło lub klucz trzeba natychmiast unieważnić i wygenerować nowe, a sekrety trzymać poza repozytorium (np. w zmiennych środowiskowych lub menedżerze sekretów).
