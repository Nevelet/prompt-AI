Genera una serie di flashcard in formato Markdown compatibili con il plugin Spaced Repetition di Obsidian, seguendo queste regole:

- Ogni flashcard deve essere formattata in Markdown.
- Usa il formato domanda → risposta con `?` e `::`, esempio:
	- `Qual è la capitale della Francia? :: Parigi`
- Per le flashcard a risposta inversa, aggiungi `:::`, esempio:
	- `Quali sono i colori primari? ::: Rosso, Blu, Giallo`
- Per le flashcard a completamento, usa ==== per nascondere una parte del testo, esempio:
	- `La teoria della relatività è stata formulata da ==Albert Einstein==`
- Per formattare le risposte, puoi usare **grassetto**, _corsivo_ e `codice inline`.
- Se necessario, aggiungi immagini con `![](URL_immagine)`.
- Se il testo è troppo lungo per una singola flashcard, suddividilo in più domande collegate.

Esempio di output:


# Storia
Quale anno è iniziata la Seconda Guerra Mondiale? :: 1939

---

# Scienza
La molecola dell'acqua è composta da quali elementi? ::: Idrogeno, Ossigeno

---

# Informatica
Il comando per visualizzare la lista dei file in una directory in Linux è? :: ls

---

# Letteratura
L'autore di "1984" è ==George Orwell==


