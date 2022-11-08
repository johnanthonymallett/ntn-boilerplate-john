<template>
  <main>
    <section class="self-center flex flex-col flex-1 items-center justify-center tracking-tight">
      <h1 class="title text-center">

        <vue-typer style="color: #FFFFFF"
          :text='["fonts","web","print"]'
          :repeat='Infinity'
          :shuffle='false'
          initial-action='typing'
          :pre-type-delay='150'
          :type-delay='150'
          :pre-erase-delay='2000'
          :erase-delay='250'
          erase-style='backspace'
          :erase-on-complete='false'
          caret-animation='blink'
        >
        </vue-typer>
      </h1>
      <h2 class="subtitle text-center">John Anthony Mallett</h2>
    </section>


  </main>
</template>