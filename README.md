# llm-agents

Interaktywny **symulator wzorców agentowych** w jednym pliku HTML — bez zależności i bez prawdziwych wywołań LLM.
Otwórz `index.html` w przeglądarce (albo włącz GitHub Pages dla tego repozytorium).

## Wzorce

| # | Wzorzec | Co pokazuje |
|---|---------|-------------|
| 1 | Łańcuch promptów | stała sekwencja wywołań LLM + programowa bramka odsyłająca do poprawki |
| 2 | Routing | tani klasyfikator kieruje zgłoszenia do specjalistów lub do człowieka (próg pewności) |
| 3 | Równoległość | sekcjonowanie (odpowiedź + guardrail + styl) oraz głosowanie większościowe |
| 4 | Orkiestrator i wykonawcy | dynamiczny plan podzadań, delegacja, ponawianie błędów, synteza |
| 5 | Ewaluator i optymalizator | pętla generuj → oceń z progiem akceptacji i limitem iteracji |
| 6 | Autonomiczny agent (ReAct) | myśl → akcja → obserwacja, błędy narzędzi, budżet kroków, zgoda człowieka |

## Funkcje

- animowany diagram przepływu wiadomości między węzłami (LLM, narzędzia, bramki, człowiek),
- ślad wykonania z czasem symulowanym, metryki: wywołania LLM, tokeny, czas, koszt (umowne),
- parametry każdego wzorca (prawdopodobieństwa błędów, progi, limity), ziarno losowości dla powtarzalności,
- sterowanie: start / pauza (spacja), praca krokowa, prędkość 0,25–4×,
- karta „Frameworki dla tego wzorca”: LangChain, LangGraph, LlamaIndex, CrewAI, AutoGen, DSPy, Claude Agent SDK, OpenAI Agents SDK i inne — z konkretnym API realizującym dany wzorzec,
- motyw jasny / ciemny, układ responsywny.
