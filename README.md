# Comprendre le hook "useState"

Alors, c'est quoi un hooks ?

## Origine

Les hooks sont des fonctions apparue avec la version 16.8 de React. Ils sont simplement des fonctions qui permettent de bénéficier de fonctionnalités de React.

## Les hooks

### useState

Le state c'est quoi ?

Le state c'est un objet qui contient des données qui vont être utilisées par notre composant. Il est possible de modifier ces données en utilisant la fonction `setState`.

#### Exemple

```js
import React, { useState } from "react";

const App = () => {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>Vous avez cliqué {count} fois</p>
      <button onClick={() => setCount(count + 1)}>Cliquez ici</button>
    </div>
  );
};
```

#### Explication

`useState` est une fonction qui prend en paramètre la valeur initiale du state. Elle retourne un tableau avec deux éléments :

-   Le premier élément est la valeur du state
-  Le second élément est une fonction qui permet de modifier la valeur du state

Dans notre exemple, `count` est la valeur du state et `setCount` est la fonction qui permet de modifier la valeur du state.




