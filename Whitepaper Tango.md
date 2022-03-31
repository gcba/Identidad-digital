# Whitepaper Tango[^1]

## Identidad Auto-Soberana: Fundamentos de un Nuevo Ecosistema Digital Descentralizado

_Buenos Aires, Argentina_

V. 0.1

10/3/2022

1. **[Resumen](#1-resumen)**

2. **[Introducción](#2-introducción)**

   2.1. [¿Por qué? La motivación](#21-por-qué-la-motivación)

   2.2 [¿Para qué? El propósito / Los beneficios esperados](#22-para-qué-el-propósito--los-beneficios-esperados)

   2.3 [¿Cómo? El enfoque propuesto](#23-cómo-el-enfoque-propuesto)

   2.4 [¿Qué? Lo que proponemos hacer](#24-qué-lo-que-proponemos-hacer)

   2.5 [¿Para quién? Audiencia](#25-para-quién-audiencia)

3. **[Trabajos preexistentes](#2-trabajos-preexistentes)**

   3.1 [W3C &amp; Decentralized Identity Foundation](#31-w3c--decentralized-identity-foundation)

   3.2 [Sovrin Foundation](#32-sovrin-foundation)

   3.3 [Hyperledger Aries &amp; Ursa &amp; Indy](#33-hyperledger-aries--ursa--indy)

   3.4 [Trust Over IP (ToIP)](#34-trust-over-ip-toip)

   3.5 [Ethereum community (ENS / EIPs)](#35-ethereum-community-ens--eips)

   3.6 [Proyecto DIDI](#36-proyecto-didi)

   3.7 [Proof Of Humanity](#37-proof-of-humanity)

   3.8 [Estado de Colorado](#38-estado-de-colorado)

   3.9 [Unión Europea](#39-unión-europea)
   
   3.10 [IDunion](#310-idunion)

4. **[Conceptos de Identidad Auto-Soberana](#4-conceptos-de-identidad-auto-soberana)**

   4.1 [Terminología](#_9ak0sa70kj7r)

   - [Identificador descentralizado o DID (por sus siglas en inglés)](#41-terminología)

   - [Sujeto de un DID (DID Subject)](#sujeto-de-un-did-did-subject)

   - [Métodos DID (DID Methods)](#métodos-did-did-methods)

   - [Documentos DID](#documentos-did)

   - [Registros de datos verificables](#registros-de-datos-verificables)

   - [DID resolvers y resolución de un DID](#did-resolvers-y-resolución-de-un-did)

5. **[Arquitectura de la Solución](#5-arquitectura-de-la-solución)**

   5.1 [Nivel 1: Identificadores Descentralizados (DIDs)](#51-nivel-1-identificadores-descentralizados-dids)

   - [Identificadores descentralizados, distintas implementaciones](#identificadores-descentralizados-distintas-implementaciones)

   - [DID Methods](#did-methods)

   - [Temas a profundizar en la fase de co-creación del whitepaper:](#temas-a-profundizar-en-la-fase-de-co-creación-del-whitepaper)

     5.2 [Nivel 2: billeteras y agentes digitales](#52-nivel-2-billeteras-y-agentes-digitales)

     5.3 [Nivel 3: intercambio y verificación de credenciales](#53-nivel-3-intercambio-y-verificación-de-credenciales)

     5.4 [Nivel 4: aplicaciones](#54-nivel-4-aplicaciones)

6. **[Estrategia de Adopción](#6-estrategia-de-adopción)**

- **[Anexo I](#anexo-i)**

- **[Anexo II](#anexo-ii)**

- **[Glosario](#glosario)**

## 1. Resumen

En el mundo digital es frecuente escuchar que la tenencia de datos otorga poder a quien los controla. La información identitaria, en especial, es quizás el registro de datos más trascendental relativo a un individuo u organización que existe. Sin embargo, hoy el acceso y uso de estos registros está fuera del control de los individuos a los que identifican. El poder y control está del lado de los entes que guardan la información, no sobre quienes refieren. El verdadero portador de la identidad queda relegado, sin noción de dónde se encuentra su información, quiénes tienen acceso a ella ni para qué es utilizada. Es por esto que, desde el GCBA, invitamos a la comunidad a co-crear un nuevo protocolo de identidad digital y auto-soberana con el usuario en el centro y al mando de su información.

El objetivo es construir un ecosistema de interacciones digitales sobre la base del protocolo de identidad digital auto-soberana consensuado con la comunidad. Buscamos facilitar la utilización del protocolo por parte de una masa crítica de usuarios para que luego el ecosistema tome vida propia de manera descentralizada. Nos imaginamos un nuevo paradigma que permita transacciones ágiles, simplificando procesos burocráticos, tanto entre actores privados como con actores gubernamentales. Hacerlo empoderará a los individuos, les dará control sobre su información y quién accede a ella. Los beneficios esperados incluyen una mayor soberanía de las personas sobre su información, una devolución del tiempo hoy gastado en trámites y burocracias a las personas y una reducción de costos transaccionales a las organizaciones.

## 2. Introducción

Las siguientes secciones describirán la motivación y el objetivo del proyecto. Utilizando lenguaje llano (no-técnico) se buscará captar la mayor audiencia posible, dando un panorama claro de la dirección y alcance del mismo.

### 2.1. ¿Por qué? La motivación

_Nota: esta sección explicará en términos motivacionales el impulso del proyecto, poniendo foco en responder por qué es necesaria esta iniciativa, por qué orientarla al dominio de las identidades digitales, por qué es oportuno hacerla en este momento y por qué debe ser impulsada desde GCBA._

- Motivación: dar lugar a un nuevo paradigma en el cual las transacciones seguras sean ágiles; donde la verificación de documentación necesaria se realice de manera rápida, confiable y privada. Este paradigma se monta sobre el principio de que las personas son quienes controlan su identidad, y son ellas quienes deciden dónde está alojada su información y quién puede acceder a ella.

- Hoy en día, la información identitaria se gestiona según el paradigma de datos centralizados. Los registros y documentos son manejados por grandes organizaciones, gubernamentales y privadas, y son éstas quiénes poseen la potestad absoluta para emitir, leer, modificar o eliminar información. Las personas no tienen control sobre su propia identidad ni pueden elegir quién tiene acceso a su información, y dependen directamente de un tercero que, como todos, siempre puede fallar. La situación actual lleva a que individuos incluso acepten condiciones sin conocer sus detalles o incluso mejores alternativas. La dependencia excesiva de unos pocos entes centralizados junto a la ampliamente conocida relevancia y poder de los datos en el siglo XXI vuelven al paradigma actual uno anticuado y riesgoso.

- En una interacción entre dos partes, conocer y verificar las identidades de las partes involucradas es condición necesaria para la construcción de un vínculo de confianza. Este vínculo es un aspecto fundamental de las relaciones sociales, comerciales y público-privadas. El primer paso de toda interacción es siempre verificar la identidad de las partes involucradas. Ya sea para registrar una nueva compañía, abrir una cuenta bancaria, anotarse en un club o contratar un servicio. Cuanto menos confianza tengan las partes, más riesgosa y menos deseable será la interacción.

- Estas transacciones también suelen requerir la presentación de documentación adicional, proceso que suele ser ineficiente y hoy ocupa mucho tiempo de las personas. ¿Qué si pudiéramos cambiar esta realidad? Hoy existe la tecnología para hacerlo. Proponemos cambiar el proceso actual de presentar documentación por otro dónde los individuos únicamente autorizan a un interesado a verificar automáticamente el cumplimiento de condiciones a través de un canal seguro. Este cambio llevaría a una enorme reducción de tiempo en las transacciones, a la vez que elevaría su confiabilidad y seguridad. En un mundo hiperconectado donde lo digital ocupa cada vez más espacio en nuestras vidas, es fundamental que se generen mecanismos confiables, seguros, abiertos y ágiles para interactuar digitalmente con lo que nos rodea sin correr riesgos.

- La existencia de una identidad digital gobernada por las personas y respaldada por un estado posibilitará nuevos escenarios de uso y, entre otras cosas, elevará la confiabilidad y la sustentabilidad en el tiempo. Los mayores beneficios se darán cuando el ecosistema se expanda por la creación de identidades digitales por parte de organizaciones privadas, gane volumen por el incremento de interacciones entre privados y se nutra de la creación de nuevas aplicaciones para canalizar transacciones entre privados. Con este protocolo se abren infinitas puertas a terceros para que desarrollen nuevas tecnologías sostenidas en la identidad, ahora de forma segura, ágil y abierta.

- Si bien existen numerosos intentos de implementar sistemas de identidad digital y auto-soberana, el componente intrínsecamente comunitario de este concepto implica la necesidad de una masa crítica de usuarios para su real y efectivo funcionamiento. Es por esto que un estado, dada sus facultades institucionales, es probablemente el mejor organismo para dar un puntapié inicial a este nuevo paradigma, garantizando una adopción masiva a través de la implementación oficial del sistema. Una vez logrado esto, la sociedad en su conjunto se beneficiará, ya que será considerablemente más simple construir nuevos protocolos sobre o en paralelo a este.

- Por primera vez en la historia de la humanidad es posible crear marcos de confianza por medios puramente tecnológicos, gracias a los avances en el campo de la criptografía que aportan tecnologías como blockchain y zero-knowledge proofs, que permiten evolucionar hacia un paradigma dónde son los mismos individuos y la sociedad los garantes sociales y no unos pocos entes centralizados.

- Existe una comunidad de emprendedores y programadores argentinos que son reconocidos mundialmente por encontrarse a la vanguardia en el desarrollo de estas nuevas tecnologías, que si se complementará con un marco institucional y un accionar coordinado con los organismos del Estado, permitiría crear riqueza, empleos de alta calidad y un posicionamiento de liderazgo para nuestro país en un tema estratégico a nivel mundial.

### 2.2. ¿Para qué? El propósito / Los beneficios esperados

_Nota: esta sección explicará cuál es el propósito del proyecto, poniendo foco en explicar sus impactos y los beneficios que generará en distintas dimensiones._

- Empoderar a los individuos y evolucionar hacia un paradigma dónde los individuos y la sociedad son los garantes sociales y no unos pocos entes centralizados. Un ecosistema abierto, confiable, seguro y transparente, montado sobre una arquitectura descentralizada, donde la confianza está respaldada por la red y no por entes centralizados.

- Potenciar las relaciones entre individuos y las instituciones (públicas y privadas) basadas en la confianza, con un resguardo tecnológico respaldado por los mismos usuarios. Al hacerlo se reemplaza un paradigma regido por fronteras y estructuras de control, por uno descentralizado y fluido.

- Agilizar los tiempos de transacción al simplificar el proceso de verificación de identidad y cumplimiento de requerimientos, devolviendo así tiempo a las personas y reduciendo costos para las empresas. Eliminar la necesidad de presentar documentación, reemplazandola por una sencilla autorización a un interesado de verificar automáticamente la tenencia de una credencial que acredite el cumplimiento de una condición o acceder a información.

- Habilitar nuevas formas de hacer negocios, compartir información y brindar acceso a servicios y recursos gubernamentales. Quién quiera podrá desarrollar y construir sobre la base ofrecida por este protocolo, abriendo innumerables puertas a nuevos proyectos y metodologías que involucren a la identidad como un factor fundamental.

### 2.3. ¿Cómo? El enfoque propuesto

_Nota: esta sección explicará cómo se desarrollará y ejecutará el proyecto. El foco no estará puesto en las herramientas específicas a utilizar sino en las metodologías, protocolos y estándares a implementar._

- Un enfoque de co-creación abierta a todo aquel que quiera colaborar.

- Siguiendo los paradigmas de la identidad auto-soberana.

- Aprovechando las posibilidades que abren nuevos avances en el campo de la criptografía (Ej.: blockchain, ZKP, etc.).

- Aprovechando las capacidades del ecosistema de emprendedores y desarrolladores que existe en Argentina, tanto en el campo de la identidad auto-soberana, como en el campo de las tecnologías utilizadas en redes públicas, descentralizadas y no permisionadas.

- Aprovechando la capacidad de GCBA para impulsar la adopción masiva y lograr rápidamente una masa crítica de usuarios.

### 2.4. ¿Qué? Lo que proponemos hacer

_Nota: esta sección se enfocará en describir el objeto, los elementos que serán construidos o desarrollados como parte del alcance de esta iniciativa._

_Debe dejar en claro que el objetivo no es desarrollar identidades digitales exclusivamente para su uso en la Ciudad de Buenos Aires ni para ningún otro contexto específico, sino sentar las bases de un protocolo que pueda ser utilizado o incluso replicado por quién sea, dónde sea._

_El documento no hará énfasis en los stacks tecnológicos a utilizar, sino que planteará una solución, en la mayor medida posible, agnóstica a las herramientas empleadas para su implementación._

A priori, se identifican los elementos claves que son necesarios para cumplir con el propósito de la iniciativa:

- Un protocolo de identidad digital que permita facilitar y eficientizar la realización de trámites y todo tipo de acciones asociadas a la identidad, y a la vez de habilitar nuevas formas de compartir información y brindar acceso a servicios provistos por todo tipo de instituciones, públicas y privadas. Que sea descentralizado, público, no permisionado, abierto, extensible y capaz de interoperar con otros protocolos similares.

- Una masa crítica de identidades digitales que sirva como "bootstrapping" del ecosistema digital y le de suficiente relevancia como para atraer tanto a nuevos usuarios, como a nuevas instituciones y empresas, logrando de esta forma una dinámica que le permita sostenerse y crecer de manera autónoma.

- Una primera aplicación, patrocinada por el GCBA, que permita el acceso y la interoperabilidad entre todos los servicios que provee el gobierno a través de estándares comunes, de forma que los usuarios perciban beneficios concretos desde una etapa muy temprana.

- Un ecosistema pujante que extienda los servicios inicialmente brindados por el gobierno, para crear nuevas experiencias y mayores beneficios para las personas y organizaciones que residan, transiten u operen en la Ciudad de Buenos Aires, que luego puedan replicarse en otras jurisdicciones o entornos a nivel local, regional y global.

### 2.5. ¿Para quién? Audiencia

Este documento apunta a servir como marco de referencia para agentes gubernamentales, proveedores de software, agentes comerciales, futuros emisores de credenciales privadas, legisladores, reguladores y público en general.

## 3. Trabajos preexistentes

_Nota: esta sección hará referencia a trabajos preexistentes que se analizaron y de alguna manera se tomarán en cuenta en el diseño específico de la plataforma propuesta._

### 3.1. [W3C](https://www.w3.org/TR/did-core/) &amp; [Decentralized Identity Foundation](https://identity.foundation/)

### 3.2. [Sovrin Foundation](https://sovrin.org/)

### 3.3. Hyperledger [Aries](https://www.hyperledger.org/use/aries) &amp; [Ursa](https://www.hyperledger.org/use/ursa) &amp; [Indy](https://www.hyperledger.org/use/hyperledger-indy)

### 3.4. [Trust Over IP](https://trustoverip.org/) (ToIP)

### 3.5. Ethereum community ([ENS](https://ens.domains/es/) / [EIPs](https://eips.ethereum.org/EIPS/eip-1484))

### 3.6. [Proyecto DIDI](https://didi.org.ar/)

### 3.7. [Proof Of Humanity](https://www.proofofhumanity.id/)

### 3.8. [Estado de Colorado](https://mycolorado.state.co.us/)

### 3.9. [Unión Europea](https://essif-lab.eu/#:~:text=EUROPEAN%20SELF%2DSOVEREIGN%20IDENTITY%20FRAMEWORK,Internet%20and%20in%20real%20life.)

### 3.10. [IDunion](https://idunion.org/?lang=en)

## 4. Conceptos de Identidad Auto-Soberana

_Nota: esta sección detallará todas las definiciones de términos relevantes que serán utilizados a lo largo del documento._

Según Sovrin, "identidad auto-soberana (Self-sovereign identity o SSI por sus siglas en inglés) es un término utilizado para describir el movimiento digital que reconoce que un individuo debe poseer y controlar su identidad sin la intervención de autoridades administrativas. La SSI permite a las personas interactuar en el mundo digital con la misma libertad y capacidad de confianza que en el mundo físico"[^2]. En 2016, Christopher Allen estableció los 10 principios para la identidad auto-gestionada que se han convertido en una referencia en el campo (ver [Anexo I](#anexo-i)).

### 4.1. Terminología

#### **Identificador descentralizado o DID** (por sus siglas en inglés)

Un identificador persistente y globalmente único que no requiere una autoridad de registro centralizada porque se genera y/o registra utilizando plataformas descentralizadas (Ej.: blockchain). Mientras el formato genérico de un DID se define en la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C, cada DID Method en particular define sus esquemas DID específicos. ![](RackMultipart20220326-4-1cj7fwj_html_c12c0dce6bb476cd.png)

#### **Sujeto de un DID** (DID Subject)

Según la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C, el "sujeto de un DID" es, por definición, la entidad identificada por el DID. Tanto las personas, como las organizaciones, pero también las cosas, o incluso los conceptos, podrían ser el sujeto de un DID.

#### **Métodos DID** (DID Methods)

Los métodos DID son el mecanismo mediante el cual se crea, resuelve, actualiza y desactiva un tipo particular de DID y su documento DID asociado. Si bien cada método DID tiene libertad para definir los detalles de su implementación – por ejemplo: cada método DID puede definir e implementar su propio "Registro de Datos Verificables" – los implementadores de un método DID deben respetar las especificaciones que se definen en la sección "[Methods](https://www.w3.org/TR/did-core/#methods)" de la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C.

#### **Documentos DID**

Los "documentos DID" contienen información asociada con un DID. Por lo general, expresan métodos de verificación, como claves públicas de criptografía asimétrica y "end-points" a servicios relevantes para las interacciones con el sujeto DID. Las propiedades genéricas admitidas en un documento DID se especifican en la sección "[Core Propoerties](https://www.w3.org/TR/did-core/#core-properties)" de la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C.

#### **Registros de datos verificables**

Un sistema que permite registrar los DIDs y la información necesaria para producir sus "documentos DID" asociados. Estos registros típicamente utilizan algún tipo de almacenamiento descentralizado que permita la verificación de los datos sin necesidad de tener una autoridad de registro (Ej.: blockchain).

#### **DID resolvers y resolución de un DID**

Un "DID resolver" es un componente con una interfaz web estándar y provisto por cada método DID que toma un DID como entrada y produce un documento DID conforme al estándar [DID-CORE](https://www.w3.org/TR/did-core/) como salida. Este proceso se denomina resolución del DID. Los pasos para resolver un tipo específico de DID están definidos por la especificación de cada método DID en particular.

## 5. Arquitectura de la Solución

_Nota: en esta sección se describe la arquitectura de la solución, incluyendo la dimensión de tecnología, pero también la dimensión del governance. Esta descripción busca ser agnóstica respecto de implementaciones tecnológicas particulares, apoyarse en estándares de la industria y enfocarse en describir los requerimientos para cada componente de la arquitectura._

La arquitectura propuesta toma como base el modelo desarrollado por la fundación "[Trust Over IP](https://trustoverip.org/)"[^3], pero con algunas extensiones y modificaciones que se consideran necesarias, por un lado para adaptar dicho modelo a las necesidades específicas de esta iniciativa, pero a la vez para incluir conceptos originados en otros trabajos preexistentes dentro del campo de la identidad digital que enriquecerán la arquitectura propuesta y permitirán ampliar su alcance a un público más grande y a una mayor diversidad de escenarios de uso.

El modelo de [ToIP](https://trustoverip.org/toip-model/) consolida mucho del conocimiento y los componentes tecnológicos generados en [trabajos preexistentes](#_s5t6sqpbn8yr) dentro del campo de la identidad digital auto-soberana, dado que la Fundación ToIP trabaja en estrecha colaboración con otras organizaciones de desarrollo de estándares, fundaciones y consorcios de la industria, para combinar sus estándares abiertos, arquitecturas y protocolos en un stack completo y coherente que permita crear una "infraestructura de confianza digital"; a escala de Internet.

El modelo de [ToIP](https://trustoverip.org/toip-model/) está organizado en cuatro niveles, cada uno de los cuales tiene una dimensión de governance y una dimensión tecnológica, y se enfoca en resolver una problemática específica:

- Nivel 1: [**identificadores descentralizados (DIDs)**](https://www.w3.org/TR/did-core/#architecture-overview)
- Nivel 2: **billeteras y agentes digitales**
- Nivel 3: **intercambio y verificación de credenciales verificables**
- Nivel 4: **ecosistemas de confianza digital**

En cada uno de los 4 niveles del modelo "ToIP" existen especificaciones y tecnologías que permiten su implementación y surgen definiciones de solución que deben ser abordadas. A continuación se presentan brevemente tanto las tecnologías a utilizar en cada nivel, como las definiciones críticas que es necesario abordar para lograr un diseño que responda a las necesidades específicas de esta iniciativa.

### 5.1. Nivel 1: Identificadores Descentralizados (DIDs)

En este nivel se aborda toda la problemática relacionada con un nuevo tipo de identificadores descentralizados, persistentes, globalmente únicos e interoperables, que se generan y verifican criptográficamente y por lo tanto no requieren ni autoridades de registro centralizadas, ni proveedores de servicios centralizados.

En este nivel se implementa un conjunto de servicios públicos y abiertos, necesarios para crear, administrar, resolver y verificar los identificadores descentralizados, que constituyen las raíces criptográficas sobre las que luego se apoya toda la construcción de la "identidad digital auto-soberana".

#### **Identificadores descentralizados, distintas implementaciones**

En los últimos años se han desarrollado distintas aproximaciones a la problemática de identificadores únicos y descentralizados. Solo para citar alguno de ellos, podemos nombrar los siguientes:

- W3C Decentralized Identifiers ([DIDs](https://www.w3.org/TR/did-core/))
- Key Event Receipt Infrastructure ([KERI](https://keri.one/))
- Ethereum Name Service ([ENS](https://ens.domains/))

Si bien todos estas aproximaciones cubren, en alguna medida, los requerimientos de nuestra iniciativa, nuestra propuesta es implementar inicialmente el nivel 1 del modelo siguiendo la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C, dado que:

- Por un lado brinda mejor cobertura a los requerimientos específicos de esta iniciativa y, por otro lado, porque es la que se encuentra más avanzada y la que está siendo más ampliamente adoptada por distintos gobiernos, organismos multilaterales y ecosistemas digitales alrededor del mundo.
- Adicionalmente, muchas de las otras aproximaciones están confluyendo hacia la especificación [DID-CORE](https://www.w3.org/TR/did-core/) del W3C, lo cual facilitará la interoperabilidad en un futuro cercano. Por ejemplo: por el lado de KERI, este ya fue incorporado como un grupo de trabajo en la [Decentralized Identity Foundation](https://identity.foundation/) y se está creando un nuevo método DID bajo el nombre de [did:keri](https://identity.foundation/keri/did_methods/), y por el lado de ENS, [Veramo](https://veramo.io/) ([Ex uPort](https://www.uport.me/)) está implementando otro método DID ([did:ens](https://github.com/veramolabs/did-ens-spec)) que permite generar dinámicamente un DID y su correspondiente DID Document para cada nombre publicado en ENS utilizando los datos almacenado en dicho registro y lo ha registrado como did:ens en el [W3C DID registry](https://www.w3.org/TR/did-spec-registries/#did-methods)

#### **DID Methods**

Los [métodos DIDs](#_1jz99r2mnluw) representan el componente central en la implementación de este nivel del modelo, y una de las decisiones más críticas en este sentido es la definición de qué métodos DID serán soportados por la plataforma para cada escenario en particular, concretamente: qué métodos DIDs serán soportados para administrar DIDs generados en esta plataforma y qué métodos DID serán soportados sólo en modalidad resolución (sólo lectura) para efectos de compatibilidad e interoperabilidad con otras plataformas similares.

Es importante destacar que no hay una única implementación de un método DID, sino múltiples implementaciones que cumplen con la especificación [DID-CORE](https://www.w3.org/TR/did-core/) y que están optimizadas y personalizadas para distintos requerimientos. A la fecha, hay más de 70 métodos DID registrados en el [W3C DID registry](https://www.w3.org/TR/did-spec-registries/#did-methods), y seguramente ese número seguirá creciendo aceleradamente en el futuro próximo.

Si bien, en teoría, las plataformas de identidad digital descentralizada deberían poder manejar todas las implementaciones de métodos DID sin un esfuerzo adicional, en la práctica, dado que [DID-CORE](https://www.w3.org/TR/did-core/) es un estándar que permite ciertas extensiones, cada método DID presenta particularidades y su integración a la plataforma requiere un esfuerzo considerable.

##### **DID Manager**

En este componente, es donde serán registrados los métodos DID soportados por la plataforma en "modalidad de gestión", es decir aquellos métodos DID que estarán habilitados para crear, actualizar y desactivar los DIDs en esta plataforma.

En un principio el DID Manager implementará el método Peer DID (did:peer), para manejar interacciones privadas entre dos partes y un método DID propio de la plataforma, que será público y basado en un [Registro de Datos Verificables](#_gb09ixlkcc8p), para ser utilizado en situaciones donde existe un número desconocido de partes (por ejemplo, el público global o algún subconjunto del mismo).

Más abajo, en esta sección, se brindan detalles de los dos métodos DID que serán soportados desde el inicio por nuestra plataforma.

##### **Universal DID Resolver**

Si bien la Decentralized Identity Foundation mantiene un servicio público y abierto, conocido como Universal Resolver (dev.uniresolver.io), cuyo propósito es brindar un único punto de acceso a los [DID Resolvers](#_la95mvstkhvg) provistos por cada uno de los métodos DID auto-registrados con dicho servicio, una práctica común, debido a las particularidades que presentan los diferentes métodos DIDs, es que cada plataforma implemente su propio Universal Resolver, para brindar, no solo un único punto de acceso a los resolvers, sino además homogeneizar la interacción con los métodos DID soportados por el Universal Resolver, ocultando la complejidad a los usuarios que se derivan de las particularidades de cada método DID.

En este componente, es donde serán registrados los métodos DID soportados por la plataforma en "modalidad solo de resolución". En un principio, sólo se implementará soporte para el método DID que será creado específicamente para esta plataforma, luego, en forma gradual, se podrán ir registrando métodos DID adicionales para ampliar la interoperabilidad y compatibilidad con DID generados en otras plataformas de identidad digital descentralizada. El método Peer DID no se incluye en el Universal Resolver, porque su resolución es privada entre las partes y solo las partes tienen acceso a los DID Documents generados por ese método.

##### **Peer DID (did:peer)**

Este método tiene la particularidad de que no requiere un [Registro de Datos Verificables](#_gb09ixlkcc8p), dado que está optimizado para situaciones donde solo intervienen dos partes que se conocen y tienen relación directa, por lo que está destinado a ser económico, rápido, escalable, seguro y muy privado.

Puede decirse que Peer DIDs son a los DID públicos basados en un [Registro de Datos Verificables](#_gb09ixlkcc8p), lo que construcciones como Ethereum Plasma, los State-Channels o Lighting Network son para las transacciones on-chain, es decir, mueven la mayor parte de las interacciones off-chain, para aumentar la escalabilidad y la privacidad, pero ofrecen opciones para volver a conectarse on-chain según sea necesario.

Para más información sobre el método Peer DID, puede consultarse la especificación en el siguiente link: [https://identity.foundation/peer-did-method-spec/](https://identity.foundation/peer-did-method-spec/)

##### **TANGO DID (did:tbd)**

Para cubrir situaciones que requieran crear y administrar DIDs dentro de nuestra plataforma y en escenarios que involucren a tres o más partes (Ejemplo: credenciales verificables) se creará un método DID propio de nuestra plataforma, el cual será registrado formalmente en el [W3C DID registry](https://www.w3.org/TR/did-spec-registries/#did-methods) para que sea reconocido a nivel global.

La creación de un método DID propio permitirá ajustar sus características a los requerimientos específicos de esta iniciativa, en particular, se pondrá especial atención a crear un mecanismo de mitigación de spam y ataques de denegación de servicio que sea apropiado para una implementación de esta naturaleza, concretamente, un mecanismo que sea eficaz para mitigar este tipo de ataques, pero que a la vez no tenga costos por transacción elevados por transacción, particularmente en situaciones donde se deba incorporar un volumen alto de identidades genuinas en un período corto de tiempo, como podría ser en la carga inicial de las identidades cuando se incorpore, por ejemplo, una nueva jurisdicción.

La creación de este método DID no será realizada desde cero, sino tomando como base las definiciones y los componentes tecnológicos disponibles de algún otro método DID que haya sido probado en experiencias anteriores y se ajuste a las necesidades propias de esta iniciativa. Existen al menos tres iniciativas que tienen un track record sólido y que podrían servir como base para crear nuestro propio método DID:

- Sovrin: creado por la [Sovrin Foundation](https://sovrin.org/) quien a su vez es uno de los miembros fundadores de la Decentralized Identity Foundation y uno de los actores más influyentes en los desarrollos que se realizaron dentro del marco del DIF/W3C.
- ETHR: creado originalmente por uPort, una empresa del grupo Consensys, otro de los miembros fundadores de la Decentralized Identity Foundation y que también tuvo gran influencia que se realizaron dentro del marco del DIF/W3C.
- Sidetree: es una iniciativa que surgió ya dentro de la Decentralized Identity Foundation que, por tratarse de una iniciativa más moderna, no solo aprovecha los aprendizajes de experiencias previas en iniciativas como Sovrin y ETHR, sino también los avances que hubo en los últimos años en los protocolos blockchain, particularmente los referidos a protocolos de segundo nivel.

De estas tres iniciativas, consideramos que SOVRIN, aún cuando es una experiencia muy valiosa, no puede ser tomada como base porque requieren: o bien montarse sobre la red Sovrin, o desplegar una nueva red usando Hyperdleger Indy, y en ambos casos serían redes permisionadas, lo cual colisiona con uno de los principios fundamentales de nuestra iniciativa de ser pública, abierta y no-permisionada.

En función de eso, las dos alternativas a evaluar serían:

1. Desplegar el método DID utilizando ETHR sobre un protocolo de nivel 2 en alguna red que sea EVM compatible, para tener niveles de escalabilidad y costos compatibles con los requerimientos de esta iniciativa.
2. Desplegar el método DID utilizando Sidetree como base en una red blockchain y una red IPFS que deberán ser definidas al momento de realizar la especificación detallada de la implementación.

Cada una de estas dos opciones tiene sus ventajas y desventajas, que deberán ser estudiadas en detalle antes de definir cuál es la opción más conveniente para esta iniciativa. De manera muy resumida, podemos decir que:

- **ETHR** , por el simple hecho de ser una implementación más antigua, tiene muchas más implementaciones, tiene abundante documentación y cuenta con un ecosistema más amplio de desarrolladores con experiencia. Por otra parte, por la misma razón de haber sido pionera, presenta algunos problemas estructurales en su diseño, lo cual limita su funcionalidad y su desarrollo a futuro. Un aspecto favorable de ETHR es que no requiere el despliegue de nodos de ningún tipo, solo desplegar los smart contracts asociados al método en alguna red compatible con EVM.
- **Sidetree** , al ser una implementación más moderna, que recoge experiencias anteriores y avances en la tecnología de base, tiene un diseño mucho más eficiente y con mayor potencial de desarrollo a futuro, está siendo apadrinada directamente por la Decentralized Identity Foundation y siendo adoptada por actores muy influyentes (Ej.: Microsoft). A la vez, por las mismas razones, no cuenta con tantas implementaciones, la documentación es incompleta y el ecosistema de desarrolladores con experiencia es limitado. Una consideración importante a tener en cuenta con Sidetree es que, aunque es un protocolo que se ancla en una red blockchain subyacente y aprovecha el mecanismo de consenso de la misma, requiere el despliegue de nodos tanto para el protocolo Sidetree, como para la red IPFS que se utilice para almacenar la información, esta característica puede ser una ventaja en algunos casos, pero requiere un mayor esfuerzo para crear el ecosistema de nodos que darán soporte a la red.

#### **Temas a profundizar en la fase de co-creación del whitepaper:**

- Mecanismos de recuperación de identidad
- Rotación de claves y resolución de DIDs
- Proof of Existence
- Buenas prácticas de seguridad

  1.

### 5.2. Nivel 2: billeteras y agentes digitales

Este nivel aborda la problemática de las billeteras y agentes digitales necesarios para aceptar, almacenar e intercambiar credenciales digitales sobre protocolos estándares de comunicación entre pares (P2P). El objetivo de este nivel es crear un espacio seguro y privado para todas las interacciones digitales que puedan ocurrir ya sea entre individuos, empresas, gobiernos o cualquier tipo de "cosa" con la que podamos interactuar digitalmente a través de una wallet/agente digital.

Temas a abordar:

- Custodial vs Non-custodial
- Billeteras individuales vs organizacionales
- Recuperación de identidad
- Buenas prácticas de seguridad

  1.

### 5.3. Nivel 3: intercambio y verificación de credenciales

Este nivel facilita el intercambio de credenciales verificables y pruebas criptográficas entre emisores, titulares y verificadores, apoyándose en protocolos estándar de intercambio de credenciales y el modelo del [triángulo de confianza de las credenciales verificables](https://trustoverip.github.io/WP0010-toip-foundation-whitepaper/trust/vcred_trust_triangle/), que permite establecer relaciones de confianza transitiva entre cualquiera de las tres partes para sus interacciones por canales digitales, de forma interoperable y a escala global.

Temas a abordar:

- Credenciales vs NFTs
- Selective disclosure
- Recuperación de identidad

  1.

### 5.4. Nivel 4: aplicaciones

Nivel 4: ecosistemas de confianza digital facilita el desarrollo de ecosistemas de confianza digital, familias completas de aplicaciones y credenciales que no solo están diseñadas para interoperar técnicamente, sino que además comparten un marco común de gobernanza del ecosistema, lo cual, entre otras cosas, permite definir modelos de información estandarizados para el conjunto de credenciales propio de cada ecosistema, lo cual habilita la interoperabilidad dentro de dichos ecosistemas.

Temas a abordar:

- Interoperabilidad

Estos principios de arquitectura son los que permitirán cumplir con los 10 principios de identidad auto-soberana (ver [Anexo II](anexo-ii)).

## 6. Estrategia de Adopción

_Nota: en esta sección se incluirán las definiciones y criterios relevantes para lograr una amplia adopción de la plataforma, contando con el respaldo e impulso que se puede dar desde el GCBA_

Algunos pasos básicos del camino a seguir

1. Co-creación de las definiciones acerca del protocolo y los estándares a emplear.
2. Desarrollo de la infraestructura tecnológica requerida.
3. Desarrollo de la primera aplicación por parte de GCBA.
4. Adopción masiva de identidades digitales impulsada por la aplicación GCBA.
5. Impulsar la adopción del ecosistema por la sociedad y actores privados.
6. Impulsar la adopción de reputaciones vinculadas a la identidad digital entre privados.

## Anexo I

A continuación se presentan los 10 principios para la identidad auto-gestionada definidos por Christopher Allen (2016)[^4]

- **Existencia.** _Los usuarios deben tener una existencia independiente_. Toda identidad auto soberana está, en definitiva, basada en el inefable "yo" presente en el corazón de la identidad. Nunca puede existir en forma enteramente digital. Este debe ser el núcleo del ser que se sostiene y apoya **.** Una identidad auto-soberana simplemente hace públicos y accesibles algunos limitados aspectos del "yo" ya existente.
- **Control.** _Los usuarios deben controlar su identidad_. Sujeto a algoritmos bien comprendidos y seguros que garanticen la validez continua de una identidad y sus atestaciones (_claims_), el usuario es la máxima autoridad sobre su identidad. Siempre deben ser capaces de referenciarla, actualizarla e incluso ocultarla. Deben poder elegir entre mantenerla privada o hacerla pública. Esto no significa que un usuario controle todas las atestaciones asociadas a su identidad: otros usuarios podrían hacer atestaciones asociadas a él/ella, pero no deben ser fundamentales para la identidad en sí.
- **Acceso** _. Los usuarios deben tener acceso a su propia información._ Un usuario debe siempre ser capaz de acceder fácilmente a todas las atestaciones e información extra asociada a su identidad. No debe haber datos ocultos ni guardianes. Esto no significa necesariamente que un usuario debe poder modificar todas las atestaciones asociadas a su identidad, pero sí que debe conocerlas. Tampoco significa que los usuarios tengan el mismo acceso a la información de los demás, sino sólo a la suya.
- **Transparencia.** _Los sistemas y algoritmos deben ser transparentes._ Los sistemas utilizados para administrar y operar una red de identidades deben ser abiertos, tanto en su funcionamiento como en su gestión y proceso de actualización. Los algoritmos deben ser libres, de código abierto bien comprendidos y lo más independientes posible de cualquier arquitectura en particular; cualquiera debe poder inspeccionar su funcionamiento.
- **Persistencia.** _Las identidades deben ser longevas._ Preferiblemente, las identidades deben durar para siempre, o al menos durante el tiempo que el usuario lo desee. Si bien se puede llegar a necesitar rotar las claves privadas y modificar cierta información, la identidad permanece. En el vertiginoso mundo de Internet, este objetivo puede no ser del todo razonable, por lo que las identidades deben durar como mínimo hasta que nuevos sistemas de identidad las vuelvan obsoletas. Esto no debe contradecir el "derecho a ser olvidado"; un usuario debe poder deshacerse de una identidad si lo desea, y las atestaciones deben modificarse o eliminarse con el paso del tiempo según convenga. Realizar esto requiere separar firmemente una identidad de sus atestaciones: no pueden estar vinculadas para siempre.
- **Portabilidad.** _La información y los servicios asociados a la identidad deben ser transportables._ Las identidades no deben estar en manos de un tercero, incluso aunque sea una entidad de confianza de la cual se espera que trabaje en el mejor interés del usuario. El problema es que las entidades pueden desaparecer - y en Internet, la mayoría acaba por hacerlo. Los regímenes pueden cambiar, los usuarios pueden trasladarse a otras jurisdicciones. Las identidades transportables garantizan que el usuario siga teniendo el control de su identidad pase lo que pase, y también pueden mejorar la persistencia de una identidad en el tiempo.
- **Interoperabilidad.** _Las identidades deben ser lo más ampliamente utilizables posible._ Las identidades tienen poco valor si sólo funcionan en nichos. El objetivo de un sistema de identidad digital del siglo XXI es hacer a la información identitaria ampliamente disponible, cruzando las fronteras internacionales para crear identidades globales, sin que el usuario pierda el control. Gracias a la persistencia y la autonomía, estas identidades ampliamente disponibles pueden volverse también continuamente disponibles.
- **Consentimiento.** _Los usuarios deben estar de acuerdo con el uso de su identidad._ Cualquier sistema de identidad se construye en torno a la puesta en común de aquella identidad y sus atestaciones, y un sistema interoperable aumenta el volumen de intercambio producido. Sin embargo, el intercambio de información sólo debe producirse con el consentimiento del usuario. Aunque otros usuarios tales como un empleador, una oficina de crédito o un amigo puedan presentar atestaciones, el usuario debe dar su consentimiento para que estas sean válidas. Tener en cuenta que este consentimiento puede no ser interactivo, pero sí debe ser deliberado y bien comprendido.
- **Minimización.** _La divulgación de las atestaciones debe ser mínima._ Cuando se revela información, esa revelación debe implicar la cantidad mínima de datos necesarios para cumplir la tarea en cuestión. Por ejemplo, si sólo se pide una edad mínima, no debe revelarse la edad exacta, y si sólo se pide una edad, no debe revelarse la fecha precisa de nacimiento. Este principio puede respaldarse en la divulgación selectiva, las pruebas de rango y otras técnicas de zero-knowledge, pero la no correlación sigue siendo una tarea muy difícil (quizás imposible); lo mejor que podemos hacer es emplear la minimalización para respaldar la privacidad lo mejor posible.
- **Protección.** _Los derechos de los usuarios deben ser protegidos._ Cuando existe un conflicto entre las necesidades de la red de identidad y los derechos de los usuarios individuales, la red debe pecar de preservar las libertades y los derechos de los individuos por encima de las necesidades de la red. Para garantizar la autentificación de la identidad debe realizarse mediante algoritmos independientes, resistentes a la censura y a la fuerza, y que se ejecuten de forma descentralizada.

## Anexo II

Mapeo de principios de diseño contra los 10 principios para la identidad auto-gestionada.

| **PRINCIPIOS PARA LA IDENTIDAD AUTO-GESTIONADA** | **PRINCIPIOS DE DISEÑO**                              |
| ------------------------------------------------ | ----------------------------------------------------- |
| EXISTENCIA                                       | _Proof of Existence_, _Proof of Humanity_             |
| CONTROL                                          | Custodial vs Non-Custodial, Recuperación de Identidad |
| ACCESO                                           | Descentralizado                                       |
| TRANSPARENCIA                                    | Co-creación, Código abierto                           |
| PERSISTENCIA                                     |
| PORTABILIDAD                                     |
| INTEROPERABILIDAD                                | Credenciales vs NFTs                                  |
| CONSENTIMIENTO                                   | _Selective Disclosure_                                |
| MINIMALIZACIÓN                                   | _Selective Disclosure_                                |
| PROTECCIÓN                                       | Estándares de seguridad                               |

## Glosario

_A COMPLETAR_

[^1]: Nombre sujeto a discusión con la comunidad.

[^2]: [Sovrin - Self-sovereign identity (SSI)](https://sovrin.org/faq/what-is-self-sovereign-identity/)

[^3]: [Trust Over IP model](https://trustoverip.org/toip-model/)

[^4]: La traducción es propia.
