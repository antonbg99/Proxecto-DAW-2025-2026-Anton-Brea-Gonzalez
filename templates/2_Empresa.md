# 1- Empresa

- [1- Empresa](#1--empresa)
  - [1.1- Idea de negocio](#11--idea-de-negocio)
  - [1.2- Xustificación da idea](#12--xustificación-da-idea)
  - [1.3- Segmento de clientes](#13--segmento-de-clientes)
  - [1.4- Competencia](#14--competencia)
  - [1.5- Proposta de valor](#15--proposta-de-valor)
  - [1.6- Forma xurídica](#16--forma-xurídica)
  - [1.7- Investimentos](#17--investimentos)
    - [1.7.1- Custos](#171--custos)
    - [1.7.2- Ingresos](#172--ingresos)
  - [1.8- Viabilidade](#18--viabilidade)
    - [1.8.1- Viabilidade técnica](#181--viabilidade-técnica)
    - [1.8.2 - Viabilidade económica](#182---viabilidade-económica)
    - [1.8.3- Conclusión](#183--conclusión)

> _EXPLICACIÓN_: Neste apartado desenvolveredes todo o referente os módulos de Empresa e iniciativa emprendedora e de FOL.

## 1.1- Idea de negocio

A idea consiste en **AutoCare Pro**, unha plataforma SaaS (Software as a Service) de xestión integral para talleres mecánicos. O **producto central** é un panel de control na nube que permite a dixitalización de orzamentos, entradas de vehículos e estados de reparación.

O **valor engadido** reside na transparencia cara ao cliente final, quen pode consultar o estado do seu vehículo en tempo real mediante un código privado. Como **producto aumentado**, ofrécese un sistema de notificacións automáticas e a posibilidade de xestión dende dispositivos móbiles (tablets) dentro do propio taller, eliminando o uso de papel.

## 1.2- Xustificación da idea

A idea xorde tras detectar que moitos talleres pequenos e medianos seguen a utilizar métodos tradicionais (papel ou follas de cálculo locais) que dificultan a comunicación co cliente e a organización interna. O **obxectivo** é profesionalizar o sector mediante unha ferramenta accesible e económica.

- **Necesidade:** Dixitalización de procesos administrativos e mellora da confianza do cliente no servizo técnico.
- **Existencia de productos:** Existen ERPs xenéricos ou softwares de automoción complexos e caros. **AutoCare Pro** consegue unha solución máis lixeira, intuitiva e centrada na comunicación co usuario.
- **Segmento:** Trátase dun sector (pequenos talleres de barrio) insuficientemente atendido por solucións de software modernas debido ao alto custo das alternativas actuais.
- **DAFO:**

  | PUNTOS FORTES | PUNTOS DEBODES |
  | :--- | :--- |
  | **Fortalezas:** Baixo custo de mantemento (Laravel), interface intuitiva, consulta en tempo real para o cliente. | **Debilidades:** Marca nova no mercado, recursos limitados para marketing inicial. |
  | **Oportunidades:** Crecente dixitalización do sector servizos, axudas estatais (Kit Dixital), ausencia de competidores áxiles na zona. | **Ameazas:** Competidores consolidados con máis funcións, reticencia ao cambio de mecánicos tradicionais. |

## 1.3- Segmento de clientes

O negocio diríxese principalmente a:

1. **Clientes:** Clientes de pequenos e medianos talleres mecánicos, de chapa e pintura ou de electricidade do automóbil que buscan modernizar a súa xestión.
2. **Usuarios:** Os mecánicos do taller (que alimentan o sistema) e os **clientes finais** do taller (propietarios de coches), que utilizan a web para consultar o estado da súa reparación.

O mercado potencial é amplo, dado que segundo o INE/IGE, o sector do mantemento de vehículos conta con miles de microempresas en Galicia que requiren solucións de baixo custo.

## 1.4- Competencia

A competencia divídese en:

- **Software especializado (Directa):** Programas como GT Estimate ou ferramentas de grandes redes de talleres. Teñen gran cota de mercado pero son complexos e de elevado custo mensual.
- **Métodos tradicionais (Substitutivos):** O uso de Excel ou axendas físicas. Están moi posicionados en talleres antigos pero son ineficientes para a xestión moderna.
- **Posicionamento:** AutoCare Pro posicionase como a alternativa **"Easy & Low Cost"**, enfocada na usabilidade por riba da cantidade excesiva de funcións.

## 1.5- Proposta de valor

**AutoCare Pro** diferénciase por:

- **Transparencia:** O portal de consulta para o cliente reduce as chamadas telefónicas preguntando "como vai o meu coche?".
- **Simplicidade:** Implementación rápida baseada en tecnoloxía web, sen necesidade de instalar software local.
- **Mellora:** Interface limpa fronte a programas de escritorio obsoletos e visualmente cargados.
- **Por que nos elixirán?** Pola facilidade de uso, a mellora da imaxe profesional que proxectan cara aos seus clientes e o prezo competitivo do servizo.

## 1.6- Forma xurídica

A forma xurídica escollida é **Empresario Individual (Autónomo)** (ou **Sociedade Limitada Unipersoal** se o investimento inicial fose maior).
Escóllese esta forma pola súa **simplicidade nos trámites de constitución** e os menores custos de xestión inicial, ideal para un proxecto de software que inicia cun único desenvolvedor.

## 1.7- Investimentos

Para poñer en marcha AutoCare Pro necesítase:

- **Equipos informáticos:** Ordenador de desenvolvemento e servidor de probas (1.200 €).
- **Infraestrutura:** Hosting anual e dominios (150 €/ano).
- **Licenzas e Software:** Ferramentas de deseño e IDEs (0 € ao usar Open Source).
- **Marketing:** Campañas en redes sociais e visitas presenciais a talleres (500 € iniciais).

### 1.7.1- Custos

- **Custos Fixos:** Autónomos (cuota reducida), hosting, conexión a internet.
- **Custos Variables:** Publicidade por clic (ADS), posibles comisións por pasarelas de pago se se integra cobro online.
- **Impostos:** IVE (21%) nas facturas e IRPF correspondente.

### 1.7.2- Ingresos

A política de prezos basearase nun modelo de **Suscrición Mensual (SaaS)**:

- **Plan Básico:** 29 €/mes para 1 taller/3 mecánicos sen pasarela de clientes.
- **Plan Premium:** 59 €/mes con funcións de notificacións SMS para os clientes.
- **Previsión:** Acadar os 20 clientes no primeiro ano de actividade.

## 1.8- Viabilidade

### 1.8.1- Viabilidade técnica

O proxecto é totalmente viable. A elección de **Laravel (PHP) + MySQL** garante unha estrutura robusta e escalable.

- **Recursos:** O equipo humano que conta cos coñecementos para a implementación.
- **Medios:** Só se require un servidor web estándar con soporte PHP, amplamente dispoñible no mercado. Non existen impedimentos técnicos graves.

### 1.8.2 - Viabilidade económica

A viabilidade económica sostense no baixo investimento inicial (asset-light). Ao ser un producto dixital, o custo de reproducilo é cero unha vez desenvolvido. Con apenas 10-15 clientes subscritos, os ingresos cubrirían os custos fixos de mantemento e seguridade social.

### 1.8.3- Conclusión

O proxecto **é viable**.
Os beneficios potenciais a medio prazo superan os custos operativos. Ademais, ao tratarse dunha solución de dixitalización, o proxecto é susceptible de recibir subvencións como o **Kit Dixital** para pemes, o que facilitaría a captación de clientes sen que estes teñan que realizar un desembolso inicial importante.

[**<-Anterior**](../../README.md)
