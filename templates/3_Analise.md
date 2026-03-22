# Requerimientos do sistema

- [Requerimientos do sistema](#requerimientos-do-sistema)
  - [1- Descrición Xeral](#1--descrición-xeral)
  - [2- Funcionalidades](#2--funcionalidades)
  - [3- Tipos de usuarios](#3--tipos-de-usuarios)
  - [4- Contorno operacional](#4--contorno-operacional)
  - [5- Normativa](#5--normativa)
  - [6- Melloras futuras](#6--melloras-futuras)

Este documento describe os requirimentos para **AutoCare Pro**, especificando as funcionalidades que ofrecerá a plataforma de xestión para talleres e o sistema de consulta para clientes finais.

## 1- Descrición Xeral

**AutoCare Pro** é unha solución SaaS (Software as a Service) deseñada para modernizar a xestión interna dos talleres mecánicos. O proxecto consiste nunha aplicación web que centraliza a información de clientes, vehículos e orzamentos, eliminando a necesidade de soportes físicos (papel).

A plataforma ofrece un panel de control privado para os profesionais do taller e unha interface pública simplificada para os clientes, permitindo que estes últimos estean informados en todo momento sobre o progreso das súas reparacións mediante un sistema de seguimento en tempo real.

## 2- Funcionalidades

A continuación detállanse as operacións principais que se poden realizar no sistema:

| Acción | Descrición | Actores | Proceso (Entrada/Saída) |
| :--- | :--- | :--- | :--- |
| **Autenticación** | Acceso seguro ao panel de xestión. | Administrador, Mecánico | **Entrada:** Email e contrasinal. **Proceso:** Verificación en BD. **Saída:** Token de sesión e acceso ao dashboard. |
| **Alta de Clientes** | Rexistro de novos propietarios de vehículos. | Administrador, Mecánico | **Entrada:** Datos persoais (DNI, telf, nome). **Proceso:** Validación e gardado en BD. **Saída:** Confirmación de rexistro. |
| **Xestión de Vehículos** | Vincular coches a clientes rexistrados. | Administrador, Mecánico | **Entrada:** Matrícula, modelo, bastidor. **Proceso:** Relación en base de datos. **Saída:** Ficha de vehículo creada. |
| **Creación de Orzamentos** | Desglose de pezas e man de obra para unha avaría. | Administrador, Mecánico | **Entrada:** Conceptos, prezos, horas. **Proceso:** Cálculo de totais e IVE. **Saída:** Documento PDF/Vista detallada. |
| **Seguimento de Reparación** | Actualización do estado do vehículo (Pendente/En curso/Listo). | Mecánico | **Entrada:** Selección de estado no panel. **Proceso:** Actualización de timestamp en BD. **Saída:** Notificación visual no sistema. |
| **Consulta Pública** | Visualización do progreso sen necesidade de login. | Cliente Final | **Entrada:** Código privado (ID reparación). **Proceso:** Búsqueda en BD por token único. **Saída:** Liña de tempo de progreso. |

## 3- Tipos de usuarios

O acceso ao sistema está definido por tres perfís claramente diferenciados:

- **Administrador (Dono do taller):** Ten acceso total. Pode xestionar a facturación, dar de alta ou baixa a outros usuarios mecánicos e configurar os datos globais do taller (logo, dirección, prezos de man de obra).
- **Usuario Técnico (Mecánico):** Ten acceso ás funcionalidades operativas. Pode rexistrar entradas de coches, crear orzamentos e actualizar o estado das reparacións, pero non ten acceso á configuración global nin a estatísticas de ingresos do negocio.
- **Cliente Final (Usuario de consulta):** Non require conta nin rexistro. Só ten acceso a unha vista de lectura mediante un código alfanumérico privado para consultar o estado do seu vehículo.

## 4- Contorno operacional

Para poder operar coa aplicación **AutoCare Pro**, os requisitos son mínimos, garantindo a súa accesibilidade:

- **Hardware:** Calquera dispositivo con capacidade de navegación web (Ordenador, Tablet ou Smartphone).
- **Software:** Navegador web actualizado (Google Chrome, Firefox, Safari ou Edge).
- **Conexión:** Acceso a internet estable para a sincronización de datos co servidor na nube.
- **Servidor (Backend):** O sistema require un contorno con PHP e base de datos MySQL (xa configurado no hosting do proxecto).

## 5- Normativa

O proxecto axústase estrictamente ás seguintes normativas legais vixentes:

- **Protección de Datos (LOPDPGDD e GDPR):** Ao xestionar datos de carácter persoal (nomes, teléfonos e matrículas), o sistema garante a confidencialidade e seguridade dos datos. Implementarase un rexistro de consentimento e a posibilidade de exercitar os dereitos de acceso, rectificación e cancelación.
- **LSSI-CE:** Cumprimento da Lei de Servizos da Sociedade da Información para as comunicacións electrónicas e avisos legais.

A aplicación contará cos seguintes apartados obrigatorios:

- **Aviso legal:** Identificando ao titular da explotación do software.
- **Política de privacidade:** Detallando que os datos se usan exclusivamente para a xestión do taller.
- **Política de cookies:** Informando sobre as cookies técnicas necesarias para a sesión de usuario.

## 6- Melloras futuras

AutoCare Pro está deseñado de xeito modular para permitir as seguintes ampliacións:

- **Pasarela de Pagos:** Integración con Stripe ou PayPal para permitir ao cliente pagar a reparación directamente dende a web.
- **Notificacións automáticas:** Envío de SMS ou correos electrónicos automáticos cando o estado do coche cambie a "Listo para entregar".
- **Estatísticas Avanzadas:** Gráficas de rendemento para o administrador (pezas máis usadas, tempo medio por reparación, etc.).
- **APP Móbil Nativa:** Desenvolvemento dunha aplicación para Android/iOS que permita o escaneo de matrículas mediante a cámara.

[**<-Anterior**](../../README.md)
