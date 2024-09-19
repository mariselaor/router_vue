<template>
  <section class="text-gray-600 body-font relative h-screen w-screen">
    <div class="absolute inset-0 h-full w-full">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d18984.348639935943!2d-89.17914842695058!3d13.63630247814398!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8f63315b733f65c3%3A0xc74a7e2b508c7a7c!2sMirador%20de%20Los%20Planes%20de%20Renderos!5e0!3m2!1ses-419!2ssv!4v1726707649162!5m2!1ses-419!2ssv"
        width="100%"
        height="100%"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
        class="opacity-75"
      ></iframe>
    </div>
    <div class="container px-5 py-24 mx-auto flex items-center justify-center h-full">
      <div
        class="bg-white rounded-lg p-6 flex flex-col w-full md:w-1/2 lg:w-1/3 relative z-10 shadow-md"
      >
        <h2 class="text-gray-900 text-xl mb-2 font-medium">Formulario de Feedback</h2>
        <p class="leading-relaxed mb-5 text-gray-600">Por favor, completa el formulario.</p>

        <div class="relative mb-4">
          <label for="email" class="leading-7 text-sm text-gray-600">Correo Electrónico</label>
          <input
            type="email"
            id="email"
            v-model="email"
            class="w-full bg-gray-100 rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-2 px-4 transition-colors duration-200 ease-in-out"
          />
        </div>

        <div class="relative mb-4">
          <label for="message" class="leading-7 text-sm text-gray-600">Mensaje</label>
          <textarea
            id="message"
            v-model="message"
            class="w-full bg-gray-100 rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 h-32 text-base outline-none text-gray-700 py-2 px-4 resize-none transition-colors duration-200 ease-in-out"
          ></textarea>
        </div>

        <button
          @click="submitForm"
          class="text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg"
        >
          Enviar
        </button>

        <p class="text-xs text-gray-500 mt-3">Gracias por tu tiempo.</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      message: '',
    }
  },
  methods: {
    submitForm() {
      if (this.email && this.message) {
        console.log('Correo Electrónico:', this.email)
        console.log('Mensaje:', this.message)
        this.email = ''
        this.message = ''
      } else {
        alert('Por favor, completa todos los campos.')
      }
    },
  },
}
</script>

<style scoped>
html,
body,
#app,
#__nuxt,
.text-gray-600 {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
}

.bg-gray-100 {
  background-color: #f7fafc;
}

.shadow-md {
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1);
}
</style>
