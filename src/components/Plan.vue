<template>
    <div>
        <div @click="seleccionar" class="plan" :class="{'plan-activo':seleccionado}">
          <div class="descripcion">
            <span class="titulo">{{ nombre}}</span>
          </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Plan',
    props: {
        nombre: {
            type: String,
            default: 'Plan 1 - Principiante',
            required: true
        }
    },
    data() {
        return {
            seleccionado: false
        }
    },
    methods: {
        seleccionar(){
            this.$emit ('select', this.nombre);
            this.seleccionado= true;
        }
    },
}
</script>

<style>

</style>