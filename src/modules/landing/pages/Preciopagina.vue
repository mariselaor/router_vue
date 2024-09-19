<template>
  <!-- component -->
  <link rel="preconnect" href="https://fonts.gstatic.com" />
  <link
    href="https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap"
    rel="stylesheet"
  />
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet" />

  <body class="font-sans bg-gray-100">
    <div class="flex flex-col items-center pt-16 pb-12">
      <div class="text-center font-semibold mb-12">
        <h1 class="text-4xl">
          <span class="text-blue-500">Planes </span>
          <span>Flexibles</span>
        </h1>
        <p class="pt-4 text-lg text-gray-500">
          Elige el plan que mejor se adapte a ti y a tu equipo.
        </p>
      </div>

      <div class="flex flex-col lg:flex-row gap-8">
        <!-- Plan Básico -->
        <div class="w-80 p-6 bg-white text-center rounded-3xl shadow-md">
          <h1 class="text-black font-semibold text-xl">Básico</h1>
          <p class="pt-2 text-2xl font-semibold">
            <span class="text-gray-400">$</span>
            10
            <span class="text-gray-400"> / usuario</span>
          </p>
          <hr class="my-4" />
          <div class="text-left space-y-4">
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              Empezar con <span class="font-semibold">mensajería</span>
            </p>
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              Reuniones de <span class="font-semibold">equipo flexibles</span>
            </p>
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              <span class="font-semibold">5 TB</span> de almacenamiento en la nube
            </p>
          </div>
          <a href="#">
            <p class="w-full py-3 bg-blue-600 text-white rounded-xl mt-6">
              <span class="font-medium">Elegir Plan</span>
              <span class="pl-2 material-icons align-middle">east</span>
            </p>
          </a>
        </div>

        <!-- Plan Estándar -->
        <div
          class="w-80 p-6 bg-gray-900 text-center text-white rounded-3xl shadow-md border-4 border-white relative"
        >
          <h1 class="text-white font-semibold text-xl">Estándar</h1>
          <p class="pt-2 text-2xl font-semibold">
            <span class="text-gray-400">$</span>
            24
            <span class="text-gray-400"> / usuario</span>
          </p>
          <hr class="my-4 border-gray-600" />
          <div class="text-left space-y-4">
            <p class="text-gray-400">
              <span class="material-icons align-middle">done</span>
              Todas las funciones del plan <span class="font-semibold">Básico</span>
            </p>
            <p class="text-gray-400">
              <span class="material-icons align-middle">done</span>
              Programación de <span class="font-semibold">llamadas flexibles</span>
            </p>
            <p class="text-gray-400">
              <span class="material-icons align-middle">done</span>
              <span class="font-semibold">15 TB</span> de almacenamiento en la nube
            </p>
          </div>
          <a href="#">
            <p class="w-full py-3 bg-blue-600 text-white rounded-xl mt-6">
              <span class="font-medium">Elegir Plan</span>
              <span class="pl-2 material-icons align-middle">east</span>
            </p>
          </a>
          <div class="absolute top-4 right-4">
            <p class="bg-blue-700 font-semibold px-4 py-1 rounded-full uppercase text-xs">
              Popular
            </p>
          </div>
        </div>

        <!-- Plan Premium -->
        <div class="w-80 p-6 bg-white text-center rounded-3xl shadow-md">
          <h1 class="text-black font-semibold text-xl">Premium</h1>
          <p class="pt-2 text-2xl font-semibold">
            <span class="text-gray-400">$</span>
            35
            <span class="text-gray-400"> / usuario</span>
          </p>
          <hr class="my-4" />
          <div class="text-left space-y-4">
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              Todas las funciones del plan <span class="font-semibold">Estándar</span>
            </p>
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              Enfoque en <span class="font-semibold">crecimiento</span>
            </p>
            <p class="text-gray-600">
              <span class="material-icons align-middle">done</span>
              <span class="font-semibold">Almacenamiento ilimitado</span> en la nube
            </p>
          </div>
          <a href="#">
            <p class="w-full py-3 bg-blue-600 text-white rounded-xl mt-6">
              <span class="font-medium">Elegir Plan</span>
              <span class="pl-2 material-icons align-middle">east</span>
            </p>
          </a>
        </div>
      </div>
    </div>
  </body>
</template>

<style scoped>
body {
  font-family: 'Montserrat', sans-serif;
}

h1 {
  font-size: 2rem;
}

button {
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #2563eb;
}
</style>
