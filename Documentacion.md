Prompts Utilizados: 
Trabajaremos un prompt para githun copilot en android studio, para trabajar una aplicacion de:
App de “¿Qué Comer Hoy?”
Descripción: El usuario toca un botón y la app le recomienda una receta al azar, usando la
API de TheMealDB .
Objetivo de aprendizaje:
● Uso de imágenes en Android (Glide o Picasso).
● Prompts para generar recomendaciones personalizadas.
● Interacción con APIs que devuelven imágenes y texto.
El enfoque principal del proyecto es aprender a formular prompts efectivos para
herramientas de IA como GitHub Copilot y Google Gemini, integrar vibecoding, y
documentar todo el proceso.














Resultados obtenidos:
Estoy creando una aplicación Android en Java con Android Studio llamada “¿Qué Comer Hoy?”.

Funcionalidad:

El usuario presiona un botón llamado “¡Sorpréndeme!”.
La app llama a la API pública TheMealDB (https://www.themealdb.com/api/json/v1/1/random.php) y muestra una receta aleatoria.
Requisitos técnicos:

Usar Retrofit con Gson para consumir la API.
Mostrar en la interfaz:
Título de la receta
Categoría
Imagen (usando Glide)
Instrucciones paso a paso
Lista de ingredientes (hasta 20 pares: strIngredient1 + strMeasure1, etc.; ignorar los nulos)
Diseño simple en un ConstraintLayout o LinearLayout con:
Un Button
Un ImageView para la foto
Varios TextView para los datos
Manejo básico de errores (por ejemplo, mostrar un mensaje si falla la red).
Todo en Java, sin usar Kotlin.
No es necesario usar ViewModel o arquitectura compleja; basta con lógica directa en MainActivity, pero con clases separadas para red y modelo.
Por favor, genera: 

La clase modelo Meal.java que represente la respuesta JSON de TheMealDB (incluye todos los campos relevantes: strMeal, strCategory, strInstructions, strMealThumb, y los 20 ingredientes y medidas).
La interfaz de Retrofit MealApiService.java.
Una clase MealRepository.java con un método getRandomMeal(Callback<MealResponse> callback).
El archivo MainActivity.java con:
Inicialización de Retrofit
Manejo del clic del botón
Llamada al repositorio
Actualización de la UI con Glide y TextViews
El layout activity_main.xml con los elementos necesarios.
Las dependencias necesarias en build.gradle (Module: app) para Retrofit, Gson, Glide y permisos de internet.

Dato Importante: Se le fue diciendo que realizara paso por paso.











Problemas encontrados: Intentamos ejecutar el programa con teléfono sin internet y nos daba error porque el teléfono no tenia acceso a internet.
También nos topamos que las recetas únicamente las da en ingles.


Reflexión Final: La experiencia de usar herramientas de IA en el desarrollo de la app “Que comer hoy” fue muy enriquecedora porque aprendimos a integrar recomendaciones inteligentes y a trabajar con Apis que devulven imágenes y texto. La IA hizo que la aplicación fuera más dinámica y útil para el usuario, pero también nos enseno que la creatividad y las decisiones del desarrollador siguen siendo claves para darle valor al proyecto.













