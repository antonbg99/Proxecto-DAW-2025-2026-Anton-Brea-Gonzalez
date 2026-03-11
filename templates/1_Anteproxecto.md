# Anteproxecto

- [Anteproxecto](#anteproxecto)
  - [1- Idea do proxecto](#1--idea-do-proxecto)
  - [2- Contextualización](#2--contextualización)
  - [3- Estudio de alternativas e viabilidade](#3--estudio-de-alternativas-e-viabilidade)
    - [3.1- Estudio de alternativas](#31--estudio-de-alternativas)
    - [3.2 Xustificación da alternativa](#32-xustificación-da-alternativa)
  - [4- Requirimentos técnicos](#4--requirimentos-técnicos)
  - [5- Planificación](#5--planificación)

## 1- Idea do proxecto

A idea do proxecto consiste no desenvolvemento dunha **páxina web de xestión integral** para talleres mecánicos, denominada **AutoCare Pro**. Trátase dunha plataforma accesible dende calquera navegador que permite aos profesionais do sector dixitalizar a xestión dos seus servizos.

A web funcionará como un panel de control onde o mecánico pode rexistrar entradas de vehículos, xerar orzamentos e actualizar o progreso das reparacións. Pola súa banda, os clientes poderán acceder a unha sección pública da web para consultar, mediante un código privado, o estado actual do seu coche, achegando transparencia e modernidade ao servizo.

## 2- Contextualización

Este proxecto responde á necesidade de moitos talleres pequenos de contar cunha presenza dixital funcional que vaia máis alá dunha simple web informativa.

- **En que consiste o proxecto?** É unha plataforma web de xestión (Backoffice) e consulta (Frontend). O propósito principal é centralizar toda a actividade do taller nunha ferramenta na nube accesible dende o ordenador do taller ou tablets.

## 3- Estudio de alternativas e viabilidade

### 3.1- Estudio de alternativas

Analizamos diversas tecnoloxías web para o desenvolvemento de **AutoCare Pro**:

| **Alternativa** | **Viabilidade técnica** | **Viabilidade económica** | **Temporalidade** | **Valoración Global** |
| ------ | ------ | ------ | ------ | ------ |
| A1 | Baixa-media (4/10): Web con Java Spring Boot + React. Spring Boot ofrece unha arquitectura sólida pero excesivamente complexa para o tempo dispoñible no ciclo de DAW. | Media (6/10): Require hosting especializado para servidores de aplicacións Java. | Viabilidade baixa (3/10): Curva de aprendizaxe moi pronunciada. | **4.5/10** |
| A2 | Media-Alta (7/10): Web con Node.js + React. Moi fluída pero require moito esforzo en configurar a seguridade e a estrutura do servidor dende cero. | Alta (8/10): Hosting económico en plataformas cloud. | Viabilidade media (7/10): Estimado en 4 meses. | **7.5/10** |
| A3 | Alta (9/10): Desenvolvemento web con PHP (Laravel) + Tailwind CSS. É a opción máis equilibrada para crear unha páxina web de xestión robusta en pouco tempo. | Alta (9/10): Hosting compartido moi barato (dende 3€/mes). | Viabilidade alta (9/10): Permite ter a web lista en 2-3 meses. | **9/10** |
| A4 | Media (7/10): Web baseada en CMS (WordPress + Plugins). Páxinas rápidas e robustas. | Alta (9/10): Moi económico. | Viabilidade alta (8/10): Moi rápido de montar pero pouco flexible. | **8/10** |

### 3.2 Xustificación da alternativa

Tras analizar os resultados, mantense a dúbida entre a **Alternativa A3 (Laravel)** e a **Alternativa A4 (WordPress)**. A decisión final dependerá do grao de personalización necesario para o sistema de xestión do taller e do tempo dedicado á codificación fronte á configuración de módulos existentes.

## 4- Requirimentos técnicos

Para que a páxina web sexa funcional e profesional, defínense os seguintes escenarios técnicos segundo a arquitectura escollida:

- **Infraestrutura Común:** Dominio (.com ou .es), hosting con soporte para PHP/MySQL e certificados SSL (HTTPS).
- **Escenario A (Laravel):**
  - **Backend:** Framework **Laravel (PHP)** para unha lóxica de negocio a medida e xestión de API.
  - **Frontend:** **HTML5**, **Tailwind CSS** e **JavaScript** (Blade templates).
  - **Bases de Datos:** **MySQL** con deseño relacional personalizado.
- **Escenario B (WordPress):**
  - **Plataforma:** Core de **WordPress** optimizado para SEO e autoxestión.
  - **Maquetación:** Uso de editores visuais (Elementor/WPBakery) e temas *responsive*.
  - **Funcionalidades:** Plugins específicos para a xestión de citas e bases de datos de clientes preconfiguradas.

## 5- Planificación

A planificación do proxecto axustarase lixeiramente dependendo da vía técnica escollida:

| Fase | Duración | Descrición (A3: Laravel / A4: WordPress) |
| --- | --- | --- |
| **Estudo e Deseño** | 3 semanas | Definición de requisitos, esquema de datos e prototipado en Figma. |
| **Implementación** | 7 semanas | **A3:** Programación desde cero da lóxica e vistas. / **A4:** Instalación, configuración de plugins e personalización. |
| **Probas e QA** | 2 semanas | Verificación de seguridade, probas de carga e corrección de bugs. |
| **Documentación e Despregue** | 2 semanas | Redacción da memoria final e subida ao servidor de produción. |

---

[**<-Anterior**](../README.md)
