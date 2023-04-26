# <h1 align=center> **Proyecto-Analitico individual Nº2** </h1>

# <h1 align=center>**`Data Analitics`**</h1>

## Introducción:

Mi nombre es Hernán Campodónico, estoy realizando una presentacion del proyecto que se realiza en los labs de Data Science de SoyHenry. 
Este proyecto busca situarnos en el rol de un Analista de Datos.
Una empresa prestadora de servicios de telecomunicaciones nos encarga la realización de un análisis completo que permita reconocer el comportamiento de este sector a nivel nacional. Considerando que la principal actividad de la empresa es brindar acceso a internet, pero también es importante considerar el comportamiento asociado al resto de los servicios de comunicación, con el fin de orientar a la empresa en brindar una buena calidad de sus servicios, identificar oportunidades de crecimiento y poder plantear soluciones personalizadas a sus posibles clientes.
Para realizarlo se nos solicito extraer informacion de la API de Enacom.

## Objetivos: 

Realizar un trabajo de ETL y EDA sobre los datasets, luego realizar un Dahsboard y un Storytelling sobre la informacion recabada y como podria ayudar a una empresa de Telecomunicaciones mejorar su servicio.
A traves de la realizacion de 4 KPIS uno debe ser:

- Aumentar en un 2% el acceso al servicio de internet para el próximo trimestre, cada 100 hogares, por provincia.


## Contenidos del Repositorio:

+ En el notebook `EDA_PA.ipynb` se encuentra analisis y ETL realizado sobre los dataset descargados.

+ En el `Analitico.pbix` se encuentra el dashboard realizado.

+ El archivo `.gitignore` se creo para cuando realice la carga de archivos en GitHub no me cargue todos los archivos si no solo los que quiero.

+ En la carpeta `Dataset_EDA-ETL` se encuentra todos los csv que utilice en el dashboard:

   - `Internet_Penetracion.csv` Penetración de Internet fijo (accesos por cada 100 hogares) : Número de accesos al servicio de Internet fijo por cada 100 hogares por provincia.

   - `Internet_Ingresos.csv`    Ingresos trimestrales por la prestación del servicio de Internet fijo : Ingresos trimestrales de los operadores por el servicio de Internet fijo.

   - `Internet_Accesos-por-tecnologia-provincia.csv` Acceso a Internet fijo por tecnología y provincia : Número de accesos al servicio de Internet fijo por tipo de tecnología en cada provincia (trimestral).

   -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

   - `telefonia_fija_ingresos.csv` Ingresos trimestrales por la prestación del servicio de Telefonia Fija : Ingresos trimestrales de los operadores por el servicio de Telefonia Fija.

   - `telefonia_fija_prov_x100.csv` Penetración de Telefonia Fija (accesos por cada 100 hogares) : Número de accesos al servicio de Telefonia Fija por cada 100 hogares por provincia.

   -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

   - `Telefonia_movil_ingresos.csv` Ingresos trimestrales por la prestación del servicio de Telefonia Movil: Ingresos trimestrales de los operadores por el servicio de Telefonia Movil.

   - `Telefonia_movil_llamadas.csv` Acceso a Telefonia Movil por llamadas y provincia : Número de accesos al servicio de telefonia movil por llamadas.

   - `Telefonia_movil_SMS.csv` Acceso a Telefonia Movil por SMS y provincia : Número de accesos al servicio de Telefonia Movil por SMS.

   - `Telefonia_movil.csv` Penetración de Telefonia Movil (accesos por cada 100 habitantes) : Número de accesos al servicio de Telefonia por cada 100 habitantes por provincia.

   -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

   - `Television_cada100.csv` Penetración de Television (accesos por cada 100 hogares) : Número de accesos al servicio de Television por cada 100 hogares por provincia.

   - `Television_ingresos.csv` Ingresos trimestrales por la prestación del servicio de Television : Ingresos trimestrales de los operadores por el servicio de Television.

   - `Television_suscripciones.csv` Acceso a Television por suspcripsiones y provincia : Número de accesos al servicio de Television pro suspcripciones.

## Herramientas utilizadas:

+ VSC.

+ Python.

+ Power bi.

## Librerias utilizadas:

- pandas - matplotlib - seaborn 

## Links:

+ Los dataset fueron extraidos de la pagina de Enacom mencionada: https://datosabiertos.enacom.gob.ar/home 

## Resumen del analisis:

Se decidio tomar un enfoque sobre la tecnologia que se deberia invertir, se analizo los ingresos anuales de todas para ver el porogreso de cada una en el periodo 2014 -2022.
Las tendencias de ingreso indicaban un aumento en internet y telefonia movil siendo los principales ingresos de una empresa de telecomunicacion. Se basa este aumento en los gustos de las nuevas generaciones donde un celular es mas comodo que una tele o un telefono fijo. Para confirmar estas tendencias se compararon donde se percibe la caida en llamadas TV envio de SMS etc. Los mismos prefieren conectarse via plataformas de mensajeria online o streaming. Por ultimo se analizo en el 2022 si se alcanzarion las metas por provincia de manterne o aumerntar un 2% los accesos por hogares. Con el mismo se percibio el aumento de infraestructura en Fibra Optica.
Mi analisis llego a la conclusion de:

- Mantener los clientes actuales y ofrecer a los nuevos clientes accesos a mayor velocidad de internet con acceso a plataformas de streaming. 

- Minutos o SMS no sirven como campaña de inversion los jovenes no les interesa eso.

- Invertir en la infrestructura de Fibra optica para las provincias con mejor acceso. Ya de por si el manteniemiento de la firba es mas facil que el coaxil o ADSL.

- En las provincias con menos acceso enfocarse en la baja competencia que se puede tener ofrecer paquetes un poco mas rapidos a menores precios que las otras empresas obtendria nuevos clientes.
  No se recomienda inversion en infraestructura en estas zonas.

### Para esto se planteron 3 KPIS con objetivos:

- Aumento de la infraestructura de un 10% de Fibra Optica, en las provincias que tenemos acceso nos va a ayudar a mantener clientes y poder ofrecerle a nuevos.

- Aumento de acceso a del 5% de los clientes en las Provincias que tenemos mas acceso. En conjunto con el KPI anterior tenemos que lograr el aumento de los clientes y mantener nuestra fidelidad con los actuales.

- Aumento del 10% de los accesos en las provincias con menos acceso. Debemos lograr con la infraestructura que tenemos ofrecer nuevos servicios que nuestros competidores no puedan alcanzar.