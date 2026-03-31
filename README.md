# 🧠 Entrenador BLD - Bot de Telegram

Un bot de Telegram automatizado con **n8n** y **Supabase** diseñado para ayudar a los *speedcubers* a practicar y memorizar pares de letras para resolver el Cubo de Rubik a ciegas (Blindfolded / BLD).

Este bot utiliza el principio de **Recuerdo Activo (Active Recall)**: te envía pares de letras de forma secuencial y evalúa tus respuestas en tiempo real, guardando tu progreso para futuras estadísticas.

## ✨ Características

* 🎮 **Entrenamiento Interactivo:** Inicia una sesión con `/empezar` y responde a los pares de letras uno por uno.
* 💾 **Memoria Persistente:** Guarda el estado de tu partida. Si te vas y vuelves, el bot sabe exactamente en qué pregunta te quedaste.
* 📊 **Registro de Errores (Próximamente Estadísticas):** Almacena un historial de todas las partidas jugadas y registra específicamente qué pares de letras fallaste para ayudarte a enfocar tu estudio.
* ⚡ **100% Automatizado:** Construido visualmente (Low-Code) usando n8n, sin necesidad de servidores complejos.

## 🛠️ Tecnologías Utilizadas

* **[n8n](https://n8n.io/):** Motor de automatización de flujos de trabajo (Workflow).
* **[Supabase](https://supabase.com/):** Base de datos PostgreSQL en la nube para guardar sesiones y progresos.
* **[Telegram Bot API](https://core.telegram.org/bots):** Interfaz de usuario a través de mensajería instantánea.

## 🕹️ Cómo usarlo

1. Entra al chat de tu bot en Telegram.
2. Escribe el comando `/empezar`.
3. El bot te lanzará el primer par (ej: **AB**).
4. Responde con tu palabra de memorización (ej: **abeja**).
5. El bot te dirá si acertaste o fallaste y te dará la siguiente pregunta hasta completar la ronda de 15.

## 🗺️ Roadmap (Próximas mejoras)

- [ ] Añadir comando `/cancelar` para abortar sesiones activas.
- [ ] Crear un comando `/estadisticas` que calcule el porcentaje de acierto histórico.
- [ ] Implementar un sistema de "Repaso Espaciado" que pregunte con mayor frecuencia las letras que más se fallan.

---
