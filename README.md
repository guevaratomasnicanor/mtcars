# mtcars
El dataset mtcars contiene información sobre 32 modelos de autos (de 1973-74) y 11 variables numéricas relacionadas con su rendimiento, consumo y diseño.
Variable	Descripción	Tipo	Ejemplo
mpg	Millas por galón (eficiencia)	numérica	21.0
cyl	Número de cilindros	numérica (entera)	6
disp	Desplazamiento (pulg³)	numérica	160
hp	Caballos de fuerza	numérica	110
drat	Relación del eje trasero	numérica	3.90
wt	Peso (miles de libras)	numérica	2.620
qsec	1/4 de milla (segundos)	numérica	16.46
vs	Motor (0 = en V, 1 = recto)	binaria	0
am	Transmisión (0 = automática, 1 = manual)	binaria	1
gear	Cantidad de marchas	numérica (entera)	4
carb	Cantidad de carburadores	numérica (entera)	4

Relaciones entre variables:
- Relaciones con la variable objetivo(mpg): Todas las variables tienen fuerte relacion con las millas por galón: Las que mas se destacan son numeros de cilindro, desplazamiento y peso (Todas impactan negativamente, con una correlacion del -85%), mientras que caballos de fuerza y tipo de motor afectan positivamente(correlacion del 68%)
- Relaciones fuertes de otras variables: 90% entre cilindros y desplazamiento, 89% entre peso y desplazamiento,83% entre cilindros y caballos de fuerza y 81% entre cilindros y motor.

INSIGHTS: - A mayor  cantidad de marchas, relacion del eje trasero y cantidad de segundos al cuarto de milla es mas probable que la marca de auto sea mas eficiente. 
- Los autos manuales o los que tienen motor recto tienen mejores rendimientos
- A menor peso, cantidad de cilindros, cantidad de carburadores,  caballos de fuerza y pulgadas de desplazamiento, menos eficiente es el auto.
 
SVM
R2 0.7039912, RMSE1.932349, MAE 1.617586
RandomForest
0.7173837, 1.888130, 1.766283
GradientBoost 0.6917919, 1.971766, 1.853657
MLP
0.4393210, 2.659442, 2.166595








