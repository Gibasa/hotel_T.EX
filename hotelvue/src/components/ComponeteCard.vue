<template>
    <div
        v-for="(accommodation, i) in $store.getters.rCard"
        :key="accommodation.id"
        class="card"
    >
        <div class="img">
            <img :src="accommodation.img" />
        </div>
        <div class="inferior-text display-g">
            <div class="inferior-text-top">
                <h3 class="titulo-h3">{{ accommodation.title }}</h3>
                <p>{{ accommodation.description }}</p>
            </div>
            <div class="inferior-text-button display-f justify-csb">
                <div class="inferior-left display-f flex-dc">
                    <div class="text2 noto-sans">A partir de</div>
                    <div class="text-valor-acomodacoes">
                        {{
                            accommodation.price.toLocaleString('pt-BR', {
                                style: 'currency',
                                currency: 'BRL',
                            })
                        }}
                    </div>
                </div>
                <div class="inferior-right display-f justify-c align-c">
                    <button
                        class="btn-blue"
                        @click="
                            this.$router.push('/reserva'),
                                changeOrder(i, accommodation.id)
                        "
                    >
                        Reservar
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ComponetCard',

    methods: {
        changeOrder: function (i, id) {
            this.$store.commit('order', i)
            if (id > 3) {
                this.counter()
            }
        },

        counter: function () {
            this.$store.commit('counter')
        },
    },
}
</script>
