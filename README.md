Fonctions de manipulation de chaînes:
- Inverser une chaîne : écrivez une fonction qui inverse une chaîne donnée.

code :
function inverserChaine(chaine) {
  return chaine.split('').reverse().join('');
}
console.log(inverserChaine("bonjour"));

- Compter les caractères : créez une fonction qui compte le nombre de caractères dans une chaîne.
  code :
  function compterCaracteres(chaine) {
  return chaine.length;
}
console.log(compterCaracteres("bonjour"));

-Mettre les mots en majuscule : implémentez une fonction qui met en majuscule la première lettre de chaque mot dans une phrase.
code :
function capitaliserMots(phrase) {
  return phrase.split(' ').map(mot => mot.charAt(0).toUpperCase() + mot.slice(1)).join(' ');
}
console.log(capitaliserMots("bonjour le monde"));

Fonctions de tableau :
- Rechercher le maximum et le minimum : écrivez des fonctions pour trouver les valeurs maximales et minimales dans un tableau de nombres.
code :
function trouverMax(tableau) {
  return Math.max(...tableau);
}

function trouverMin(tableau) {
  return Math.min(...tableau);
}
console.log(trouverMax([1, 2, 3, 4])); 
console.log(trouverMin([1, 2, 3, 4])); 

-Somme d'un tableau : créez une fonction qui calcule la somme de tous les éléments d'un tableau.
code :
function sommeTableau(tableau) {
  return tableau.reduce((somme, nombre) => somme + nombre, 0);
}
console.log(sommeTableau([1, 2, 3, 4]));

-Filtrer le tableau : implémentez une fonction qui filtre les éléments d'un tableau en fonction d'une condition donnée.
code : 
function filtrerTableau(tableau, condition) {
  return tableau.filter(condition);
}
console.log(filtrerTableau([1, 2, 3, 4], nombre => nombre > 2)); 

Fonctions mathématiques :
- Factorielle : Écrivez une fonction pour calculer la factorielle d'un nombre donné.
  code :
  function factorielle(n) {
  if (n === 0 || n === 1) return 1;
  return n * factorielle(n - 1);
}
console.log(factorielle(5));

- Vérification des nombres premiers : créez une fonction pour vérifier si un nombre est premier ou non.
  code :
  function estPremier(nombre) {
  if (nombre <= 1) return false;
  for (let i = 2; i <= Math.sqrt(nombre); i++) {
    if (nombre % i === 0) return false;
  }
  return true;
}
console.log(estPremier(7));
console.log(estPremier(10));

- Suite de Fibonacci : Implémenter une fonction pour générer la suite de Fibonacci jusqu'à un nombre donné de termes.
  code :
  function suiteFibonacci(termes) {
  const sequence = [0, 1];
  for (let i = 2; i < termes; i++) {
    sequence.push(sequence[i - 1] + sequence[i - 2]);
  }
  return sequence.slice(0, termes);
}
console.log(suiteFibonacci(10)); 

