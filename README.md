 # test-get-https
test_get_https es una aplicación que permite realizar test de los certificados agregando la dirección https y pasando el trust que deseamos probar.



## Requisitos

* JDK 1.8
* Maven

## Instalación

```bash
$ git clone PROJECT_URL
$ cd test_get_https
$ mvn clean install package 
```



## Ejemplo

```bash
$ java -jar -Djavax.net.debug=all -Djavax.net.ssl.trustStore=/opt/example.keystore -Djavax.net.ssl.trustStorePassword=user@password test_get_https-0.0.1-SNAPSHOT-jar-with-dependencies.jar https://www.example.com
```



