---
title: "Tungsten Engine"
description: "My own modern game engine!"
dateString: "Aug 2025"
draft: false
tags: ["C++", "Slang", "Vulkan", "Graphics Programming", "Game Development", "Engine Development"]
showToc: false
weight: 202
cover:
    image: "projects/tungsten-engine/cover.png"
---

## Description

Earlier this year, I decided I wanted to improve my knowledge and experience with making game engines. Previously, I only had small renderers that were able to render models,
but these weren't much optimized, nor were they extendable to the scale of a full game.

From that, I started **Tungsten Engine**, my own modern & scalable game engine. My goal with this engine is to take a step even further in the domain of game engine development,
so that I have the knowledge to work on even bigger engines in the industry.

Tungsten Engine is a **modular**, **easily extendable** and **fast** game engine made in C++. It uses **Vulkan** for the rendering, providing me access to lower-level control over
the hardware, letting me access more optimization paths for the rendering engine.

The Tungsten Engine also uses an ECS to handle interractions between systems, entities and their data, letting the developer access fast and easy scene composition.

*This is a simple description of the engine. For more details on the engine, see the [blog](https://pixfri.is-a.dev/blog/).*