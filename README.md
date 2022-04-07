# Proyecto_m3

## Modelo de Machine Learning para predecir el precio de los diamantes

### El reto:

El reto propuesto es crear un modelo de machine learning que prediga los precios de los diamantes. Para ello, se nos ha dado una base de datos con 40455 registros y 11 features. Estas features son tanto númericas como cartgeoricas, por lo que se deberán transformar las categoricas y definir el target.

### Metodología
1. **Importar librerías**: Numpy, pandas, matplotlib, sklearn, sqlalchemy, sqlite3, pickle.
2. **Acceder a la base de datos.db**: Para acceder a la base de datos de SQL se ha utilizado SQLite
3. **Instanciar las BBDD**: Para tratar la base de datos con pandas, se han instanciado en variables.
4. **Preparación de los datos**: Diferenciar entre las features categoricas, númericas y definir el target (Feature a predecir)
5. **Get dummies**: Las features categóricas se deben transformar en números para que pueda funcionar el modelo con el método get.dummies
6. **Estandarizar las features**: Para estandarizar las variables se ha utilizado el método de sklearn StandardScaler.
7. **Dividir la BBDD**: Para diferenciar que parte del modelo es de entrenamiento, y que parte de test se ha utiliazado el método train_test_split, utilizando para entrenar el 80% del modelo
8. **¿Cual es el modelo más acertado?**: Para probar distintos modelos y ver cual es el modelo que nos daba un valor de RMSE más bajo, se han probado los siguientes:
    +LinearRegression()
    +linear_model.Lasso()
    +ElasticNet()
    +Ridge()
    +SVR()
    +SGDRegressor()
    +**RandomForestRegressor()**
siendo este último el modelo que menos error daba, obteniendo como resultado del RMSE un 206€







