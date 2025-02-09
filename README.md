# Risolutore di Sudoku

Questo programma Python risolve un puzzle Sudoku 9x9 utilizzando l'algoritmo di backtracking. Data una griglia Sudoku incompleta, il programma tenta di riempire le celle vuote con numeri da 1 a 9 in modo che ogni riga, colonna e sotto-griglia 3x3 contengano tutti i numeri da 1 a 9 senza ripetizioni.

## Funzionalità

- Risolve un Sudoku 9x9 utilizzando l'algoritmo di backtracking.
- Accetta una griglia 9x9 come input, dove le celle vuote sono rappresentate da `0`.
- Modifica la griglia di input per riempire i numeri corretti.
- Restituisce `True` se è stata trovata una soluzione, e `False` se non esiste una soluzione valida.

## Esempio di utilizzo

Ecco un esempio di come utilizzare il risolutore di Sudoku con un puzzle di esempio:

```python
# Definizione della griglia Sudoku con celle vuote rappresentate da 0
griglia = [
    [7, 8, 0, 4, 0, 0, 1, 2, 0],
    [6, 0, 0, 0, 7, 5, 0, 0, 9],
    [0, 0, 0, 6, 0, 1, 0, 7, 8],
    [0, 0, 7, 0, 4, 0, 2, 6, 0],
    [0, 0, 1, 0, 5, 0, 9, 3, 0],
    [9, 0, 4, 0, 6, 0, 0, 0, 5],
    [0, 7, 0, 3, 0, 0, 0, 1, 2],
    [1, 2, 0, 0, 0, 7, 4, 0, 0],
    [0, 4, 9, 2, 0, 6, 0, 0, 7]
]

# Stampare la griglia iniziale
print("Griglia iniziale:")
stampa_griglia(griglia)

# Risolvere il Sudoku
if risolvi(griglia):
    print("Sudoku risolto!")
    stampa_griglia(griglia)
else:
    print("Nessuna soluzione trovata.")
```

## Come Funziona

1. **Verifica della validità dei numeri:**

   - Il programma controlla se un numero può essere inserito in una data posizione, verificando riga, colonna e sotto-griglia 3x3.

2. **Ricerca della prima cella vuota:**

   - Scansiona la griglia per trovare una cella con valore `0`.

3. **Backtracking:**

   - Inserisce un numero valido nella cella vuota e procede ricorsivamente fino alla soluzione completa.
   - Se non trova una soluzione valida, torna indietro e prova un altro numero.

## Requisiti

- Python 3.x

## Esecuzione

Per eseguire il programma, basta eseguire lo script Python contenente il codice.

```bash
python sudoku_solver.py
```

## Autore

Questo progetto è stato sviluppato per risolvere automaticamente Sudoku 9x9 utilizzando tecniche di backtracking.
