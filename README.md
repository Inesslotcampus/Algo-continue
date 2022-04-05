# Algo-continue

## 1. Affichage de tableaux 1D en console

__Écrire une fonction print1D qui affiche le contenu d’un tableau en console. Cette
fonction n’a pas de valeur de retour. Elle prend en paramètre d’entrée un tableau 1D.__

Mon code:

int[] tab = {0, 1};

void setup(){

  print1D(tab); 
}

void print1D(int tab[]){

  for (int i=0; i < tab.length ; i ++){
  
    println(tab[i]);

}
}


## 2. Affichage de tableaux 2D en console 

__Écrire une fonction print2D qui affiche le contenu d’un tableau en console. Cette
fonction n’a pas de valeur de retour. Elle prend en paramètre d’entrée un tableau 2D.__

Mon code: 

int[][] tab = { {0, 1}, {2, 3 } };

void setup() {

  print2D(tab);
}

void print2D(int[][] tab) {

  for (int stab [] : tab) {
  
    println('\n');
    
    for (int numb : stab) {
    
      print(numb);
    }
  }
}

## 3. Initialiser un tableau 2D diagonal 

__Écrire une fonction “ diagonal ” qui prend en paramètre un entier size et retourne
un tableau 2D.
Le tableau créé est de taille size x size
Chaque cellule vaut 0 si elle n’est pas sur la diagonale et 1 si elle est sur la diagonale.__

void setup() {

  print2D();
}
int[][] diagonal(int size) {
  int[][] array = new int[size][size];
  for (int n = 0; n<array.length; n++) {
    array[n][n]=1;
  }
  return array;
}




void print2D() {

  int[][] array=diagonal(4);
  

  for (int i=0; i<array.length; i++) {
  
    print('\n');
    
    for (int y=0; y<array.length; y++) {

      print(array[i][y]);
    }
  }
}





