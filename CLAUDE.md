# ZnanyLekarz widget — instrukcje dla Claude

## Wspólna polityka skilli
- Te same custom skills konta Claude mają być używane niezależnie od tego, czy praca odbywa się na macOS, Windows, lokalnie czy w Claude Code Cloud. Nie instaluj lokalnych duplikatów skilli, pluginów ani `.claude/skills` tylko po to, aby wyrównać środowiska.
- Własne skille konta: `sepia`, `prezentacje-medyczne`, `usg-slinianek`, `opis-usg-tarczycy`, `opis-usg-piersi`, `opis-usg-jamy-brzusznej`. Jeżeli któregoś nie widać w świeżej sesji, traktuj to jako problem synchronizacji konta lub sesji; nie twórz lokalnej kopii.
- `sepia` jest domyślną warstwą redakcyjną dla tekstu w języku naturalnym. Stosuj ją automatycznie, chyba że użytkownik wyraźnie napisze `bez Sepia`, `nie używaj Sepia` albo wyłączy ją dla wskazanej kategorii treści.
- Skill domenowy ma pierwszeństwo przed Sepia. Dla prezentacji używaj `prezentacje-medyczne`; dla odpowiedniego opisu USG używaj właściwego skilla USG. Sepia może poprawiać tylko powierzchowną warstwę językową i nigdy nie może zmieniać znaczenia, faktów, danych, liczb, jednostek, dat, nazw, cytowań, bibliografii, rozpoznania ani stopnia pewności.
- Kod, konfiguracja, polecenia terminala, JSON/YAML, dane strukturalne i tabele nie są stylistycznie przepisywane przez Sepia; naturalnojęzykowe objaśnienia wokół nich mogą z niej korzystać.
- Reguły repozytorium mogą zaostrzać bezpieczeństwo i workflow, ale nie powinny tworzyć lokalnych kopii skilli ani zmieniać tej wspólnej polityki bez wyraźnego polecenia użytkownika.

## Bezpieczeństwo repozytorium
- Pracuj tylko na plikach potrzebnych do bieżącego zadania.
- Nie umieszczaj danych pacjentów, sekretów, tokenów ani danych uwierzytelniających w repozytorium.
- Zawsze pytaj przed merge lub push do `main`, force push, zmianą historii, usuwaniem danych lub gałęzi, zmianą widoczności repozytorium oraz działaniami produkcyjnymi.
