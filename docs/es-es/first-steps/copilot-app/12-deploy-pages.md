---
title: "Lección 12 - Publica el sitio con GitHub Pages"
description: "Usa la aplicación GitHub Copilot para configurar un flujo de trabajo de Pages, revisar su solicitud de incorporación de cambios y comprobar el Space Quiz publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica el Space Quiz con GitHub Pages para que cualquiera pueda acceder a él. Copilot puede preparar el flujo de trabajo y guiarte durante la implementación, pero tú eres responsable de revisar los cambios y confirmar que el sitio está publicado.

En esta lección:

- pedirás a Copilot que configure la implementación con GitHub Pages.
- revisarás el flujo de trabajo y la solicitud de incorporación de cambios antes de combinarla.
- seguirás la implementación y comprobarás el sitio publicado.

## Escenario

El Space Quiz ya está en un repositorio de GitHub, pero quienes quieran probarlo necesitan una forma sencilla de hacerlo. Al publicar el sitio de un solo archivo con GitHub Pages, estará disponible en una URL pública sin añadir un servidor ni dependencias de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot para `space-quiz`, envía este prompt:

```plaintext
Habilita GitHub Pages para este repositorio. Crea un flujo de trabajo de GitHub Actions que compile el sitio web si es necesario y lo publique en GitHub Pages. Añade un README que describa la aplicación y cómo ejecutarla localmente si todavía no existe. Crea una solicitud de incorporación de cambios con estos cambios y combínala cuando se superen las comprobaciones obligatorias. Supervisa la implementación hasta que se complete correctamente y, después, indica la URL final del sitio web publicado. Si no tienes permiso para habilitar Pages o combinar la solicitud, dime exactamente qué debo aprobar o hacer; no informes de que se ha completado correctamente hasta que el sitio esté publicado.
```

![Diagrama en tres etapas: una solicitud de incorporación de cambios de space-quiz combinada; una ejecución correcta de GitHub Actions para implementar el sitio web, con los pasos Build website, Upload artifact y Deploy to Pages; y el Space Quiz publicado en yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pide al agente que cree y combine una solicitud de incorporación de cambios y que cambie la configuración de Pages del repositorio. Antes de continuar, revisa la diferencia, los permisos de implementación y las solicitudes de aprobación de GitHub.

## Revisa el flujo de trabajo y comprueba la implementación

1. Confirma que el README solo se añade si el repositorio aún no tiene uno.
2. Revisa los cambios de la solicitud de incorporación de cambios, incluidos los pasos de compilación e implementación del flujo de trabajo.
3. Combina los cambios solo después de que se superen las comprobaciones obligatorias de la solicitud de incorporación de cambios.
4. Sigue la ejecución de implementación de GitHub Actions hasta que se complete correctamente.
5. Abre la URL indicada y confirma que se carga el Space Quiz.

Si el agente no puede habilitar Pages o combinar la solicitud de incorporación de cambios, sigue las instrucciones específicas que te proporcione. No des la tarea por terminada hasta que la implementación se complete correctamente y se cargue el sitio publicado.

## Resumen y siguientes pasos

El Space Quiz ya está disponible como sitio publicado y has comprobado la implementación sin depender del informe del agente. Continúa con la [lección 13: Repaso y pasos siguientes][next-lesson].

[next-lesson]: ../13-review/
