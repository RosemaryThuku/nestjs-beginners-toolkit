# NestJS Modules – Beginner Guide

## Overview

In NestJS, a **module** is a class annotated with the `@Module()` decorator.
Modules help organize your application into logical parts.

Think of a module as a **folder that groups related features together**.

---

## Why Modules Matter

Modules help you:
- Keep code organized
- Separate concerns (users, auth, products, etc.)
- Control what parts of the app can access others

Without modules, large NestJS apps become messy and hard to maintain.

---

## Basic Module Example

```ts
import { Module } from '@nestjs/common';
import { AppController } from './app.controller';
import { AppService } from './app.service';

@Module({
  controllers: [AppController],
  providers: [AppService],
})
export class AppModule {}
---

## References

- [Official NestJS Docs](https://docs.nestjs.com)
- [NestJS Modules](https://docs.nestjs.com/modules)
- [NestJS Controllers](https://docs.nestjs.com/controllers)


