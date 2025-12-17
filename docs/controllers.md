# Controllers in NestJS – Beginner Guide

## Overview
Controllers handle incoming HTTP requests and return responses.

In NestJS, controllers define routes like `/users`, `/products`, etc.

## Why Controllers Matter
Without controllers:
- Your app cannot receive requests
- APIs cannot expose endpoints

## Basic Example

```ts
import { Controller, Get } from '@nestjs/common';

@Controller()
export class AppController {
  @Get()
  getHello(): string {
    return 'Hello World';
  }
}
