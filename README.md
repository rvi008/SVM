# TP SVM

## Question 1
We load the Iris Dataset and train a simple Linear Kernel SVM.
The fiting score is 66%.
We get a cross validated score of 72% +/-16% accuracy.

## Question 2
We now train a polynomial kernel SVM and get a fiting score of 72% (better) but the  cross validated score is 72% +/- 16%. No improvement

## Question 3 
La deuxième contrainte de l'équation (2) peut se réécrire\n,
    $$ \\xi_i \\geq 1-y_i(\\langle w,\\Phi(x_i) \\rangle + \\omega_0) \\;\\; \\forall i$$\n,
    \n,
    Par ailleurs la plus petite valeure de $\\xi_i$ est $0$ (première contrainte de (2)), ce qui correspond au fait que le point $i$ soit du bon côté de sa marge. On peut alors écrire:\n,
    \n,
    $$  \\xi_i \\geq \\left[1-y_i(\\langle w,\\Phi(x_i) \\rangle + \\omega_0)\\right]_+ \\geq 0 \\;\\; \\forall i$$\n,
    \n,
    Cette nouvelle contrainte inclus les deux contraintes initiales de l'équation (2).\n,
    \n,
    $\\xi_i$ étant le coût d'une mauvaise classification, on peut remplacer $\\xi_i$ par $\\left[1-y_i(\\langle w,\\Phi(x_i) \\rangle + \\omega_0)\\right]_+$ dans l'expression à minimiser. Le coût d'une mauvaise classification est alors inférieur au coût $\\xi_i$, mais les contraintes qui apparaissaient dans l'expression initiale du problème primal disparaissent (elles sont inclues dans la fonction Hinge).  \n,
    \n
