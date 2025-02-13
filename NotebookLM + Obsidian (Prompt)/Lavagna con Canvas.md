Genera una sintesi da includere in un file JSON strutturato per creare un Canvas in Obsidian, seguendo queste specifiche:

- Il file deve essere in formato JSON compatibile con Obsidian Canvas.
- Ogni nodo deve essere rappresentato con:
    - `id`: un identificatore univoco (usa un UUID o una stringa casuale).
    - `x` e `y`: coordinate per la disposizione sulla tela.
    - `width` e `height`: dimensioni della card.
    - `type`: il tipo di nodo, che può essere "text" (testo libero) o "file" (link a una nota esistente).
    - Se il nodo è di tipo "text", deve avere un campo `"text"` con il contenuto della card.
    - Se il nodo è di tipo "file", deve avere un campo `"file"` con il nome del file markdown da collegare.
- Se necessario, collega i nodi tra loro con connessioni (`connections`) e specifica il lato di collegamento (`edges`).
- Se il Canvas rappresenta una mappa concettuale, i nodi devono essere distribuiti spazialmente in modo chiaro.
- Se è un flusso sequenziale, i nodi devono essere allineati in ordine logico.

Esempio di struttura JSON valida:

```JSON
{
	"nodes":[
		{"id":"1","type":"text","text":"Questa è una card iniziale","x":-300,"y":-300,"width":320,"height":152},
		{"id":"2","type":"text","text":"Questa è un'altra card","x":160,"y":-300,"width":329,"height":111}
	],
	"connections":[
		{"from":"1","to":"2"},
		{"from":"2","to":"3"}
	],
	"edges":[
		{"id":"f3ac02f7b2ed73b2","fromNode":"1","fromSide":"right","toNode":"2","toSide":"left"}
	]
}
```