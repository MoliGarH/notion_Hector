# July hackathon - Hector

[Propuesta curso paginas web.docx](July%20hackathon%20-%20Hector/Propuesta_curso_paginas_web.docx)

### Ideas to build! 🏗️

Build a web-based app to…

- Manage classes from a teacher's perspective.
- Expenses controller dashboard.
- App to split wages

# **Web apps** vs **Desktop apps** 🤔⁉️

- They can be accessed from any platform. You only need a browser
    - Otherwise; you would need to create a Windows one, Mac, Linux.
- Easier updates for the user.
- Easier tracking.
- “”Secure”” …
- SEO
- Monitorización (Google analitycs)

# Tech Stack (for webApps) 🦀

<u>**Programing languages:**</u>

- Design:
    - HTML (5) << estructura. Como poner enlaces a otras paginas!
    - CSS
- Intelligence:
    - JavaScript

## Frontend (UI)

[Angular](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjy5cPRlNaGAxVKQPEDHTcsDGsQFnoECBUQAQ&url=https://angular.dev/&usg=AOvVaw2xYz8JY0eG2b_pcI3abwp8&opi=89978449)

[Vue.js](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi7rJDXlNaGAxVxSPEDHQGBCzIQFnoECAYQAQ&url=https://vuejs.org/&usg=AOvVaw06q0bfK8Y9QAOb2C8cD5Qh&opi=89978449)

[React](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiC373LlNaGAxUTefEDHZ0DBrEQFnoECAkQAQ&url=https://react.dev/&usg=AOvVaw1tEjYYiD7LQlxO53dgjTHV&opi=89978449)

## Backend (Server)

[Spring Boot](https://spring.io/projects/spring-boot)

[FastAPI](https://fastapi.tiangolo.com/)

[Ktor: Build Asynchronous Servers and Clients in Kotlin](https://ktor.io/)

## Storage (bbdd)

[SQLite Home Page](https://sqlite.org/)

[5.11. Table Partitioning](https://www.postgresql.org/docs/current/ddl-partitioning.html)

[MongoDB: The Developer Data Platform](https://www.mongodb.com/)

## “All in one” Frameworks

[Django](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjJqPmxk9aGAxXqRPEDHU6zARkQFnoECAYQAQ&url=https://www.djangoproject.com/&usg=AOvVaw3E6qaJashVeeIx3oahQxD7&opi=89978449)

[Ruby on Rails](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi6yq25k9aGAxXCVvEDHVewC80QFnoECAcQAQ&url=https://rubyonrails.org/&usg=AOvVaw3O0jVyoMa-kkxOw8djop2L&opi=89978449)

[Symfony, High Performance PHP Framework for Web Development](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwjR_LeYlNaGAxWcSPEDHW9YC78QFnoECCQQAQ&url=https://symfony.com/&usg=AOvVaw2jpU3WKTF0gukfwPK7uAJ1&opi=89978449)

compilador vs interprete → webkit engine (to explain)

## Referencias

[W3Schools.com](https://www.w3schools.com/html/default.asp)

```jsx
<template>
    <v-form v-model="valid" @submit.prevent="generar_tabla">
      <v-container>
        <v-row>
          <v-col cols="12" md="4">
            <v-text-field
              v-model="numero"
              :model-value="numero"
              :counter="10"
              label="Numero"
              hide-details
              required
            ></v-text-field>
            <v-btn  type="submit">Generar</v-btn>
          </v-col>
        </v-row>
        <v-list>
            <v-list-item v-for="item in resultados">
            <h3>{{item}}</h3>
            </v-list-item>
        </v-list>
      </v-container>
    </v-form>
  </template>

<script>
import { ref } from 'vue';
let number = ref(1)
let resultados = ref([])
let generar_tabla=() => {
    let numero = parseInt(number.value);
    for (let i=1;i<=10;i++){
        resultados.value.push(`${numero}x${i}=${numero*i}`);
    }
}
</script>

<style>

</style>
```