# Isogramma
Determina se una parola o una frase è un isogramma.

### Descrizione generale della consegna
La consegna consiste nel risolvere il problema dell'"isogramma". Un isogramma è una parola o una frase in cui non ci sono lettere duplicate, cioè ogni lettera appare una sola volta. 

### Soluzione utilizzata con commenti al codice

Codice scritto in C# e la soluzione proposta utilizza


```csharp 
word = word.ToLower();
for (int i = 0; i < word.Length; i++)
{
    for (int j = 0; j < word.Length; j++)
    {
         if((word[i]==word[j]) && word[i]!='-' && word[i]!=' ' && (i!=j)){return false;}
    }
}
return true;

```




