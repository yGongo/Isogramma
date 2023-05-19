# Isogramma
Determina se una parola o una frase è un isogramma.

### Descrizione generale della consegna
La consegna consiste nel risolvere il problema dell'"isogramma". Un isogramma è una parola o una frase in cui non ci sono lettere duplicate, cioè ogni lettera appare una sola volta. 

### Soluzione utilizzata con commenti al codice

Codice scritto in C# e la soluzione proposta utilizza


```csharp 
// Converto la stringa "word" in minuscolo per non considerare le differenze tra lettere maiuscole e minuscole
word = word.ToLower();

// Itero attraverso ogni carattere della stringa utilizzando un indice "i"
for (int i = 0; i < word.Length; i++)
{
    // Itero attraverso ogni carattere della stringa utilizzando un indice "j"
    for (int j = 0; j < word.Length; j++)
    {
         // Controllo se il carattere alla posizione "i" è uguale al carattere alla posizione "j"
         // e se entrambi i caratteri non sono "-" o spazi vuoti e se le posizioni "i" e "j" non sono uguali
         if((word[i]==word[j]) && word[i]!='-' && word[i]!=' ' && (i!=j))
         {
             // Se le condizioni sopra sono soddisfatte, la stringa non è un isogramma, quindi restituisco false
             return false;
         }
    }
}

// Se il ciclo termina senza trovare duplicazioni, la stringa è un isogramma, quindi restituisco true
return true;

```




