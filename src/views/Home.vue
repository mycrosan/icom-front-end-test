<template>
    <v-container fluid class="pa-0" v-wow="{ 'animation-name': 'fadeIn'}">
        <!-- primeira sessão -->
        <v-layout row wrap align-right>
            <v-flex md3></v-flex>
            <v-flex xs12 md2>
                <div class="text-md-right text-xs-center">
                    <div class="space-logo"></div>
                    <img style="width: 175px" class="logo" v-wow="{ 'animation-name': 'bounceInDown','animation-duration': '1s'}"
                         src="../assets/icom_logo.svg"
                    >
                    <v-list class="menu-container">
                        <v-list-tile v-for="item in menu" v-wow="{ 'animation-name': 'fadeInLeft','animation-duration': '1s'}">
                            <v-list-tile-content>

                                <v-list-tile-title class="text-md-right"><a>{{item.name}}</a></v-list-tile-title>

                            </v-list-tile-content>
                        </v-list-tile>
                    </v-list>
                </div>
            </v-flex>
            <v-flex xs12 md7>
                <div class="bg-img">
                    <div class="content-bg-1" v-wow="{ 'animation-name': 'fadeIn','animation-duration': '2s'}">
                        Porque Deus amou o mundo de tal maneira que deu o seu Filho unigênito, para que todo aquele que nele crê não pereça, mas tenha a vida eterna.<br>João 3:16
                    </div>

                    <img class="doodle-top" v-wow="{ 'animation-name': 'flip','animation-duration': '40s'}" src="../assets/doodle.svg">


                </div>
            </v-flex>
        </v-layout>
        <!-- segunda sessão -->
        <v-layout row wrap>
            <v-flex xs12 md3>
                <div class="bg-img-2">

                    <img class="doodle-bottom animated infinite rotateIn" style="animation-duration: 30s;" src="../assets/doodle.svg">
                </div>
            </v-flex>
            <v-flex xs12 md9>
                <v-layout row wrap align-right>
                    <v-flex md6>
                        <div class="box-1-middle" v-wow="{ 'animation-name': 'fadeInUp','animation-duration': '2s'}">
                            Bem-aventurado o homem que não anda segundo o conselho dos ímpios, nem se detém no caminho dos pecadores, nem se assenta na roda dos escarnecedores.

                            Salmos 1:1
                        </div>
                        <div class="box-2-middle" v-wow="{ 'animation-name': 'fadeInUp','animation-duration': '1s'}">
                            Então foram chamados os escrivães do rei, naquele mesmo tempo, no terceiro mês (que é o mês de Sivã), aos vinte e três dias; e se escreveu conforme a tudo quanto ordenou Mardoqueu aos judeus, como também aos sátrapas, e aos governadores, e aos líderes das províncias, que se estendem da Úndia até Etiópia, cento e vinte e sete províncias, a cada província segundo o seu modo de escrever, e a cada povo conforme a sua língua; como também aos judeus segundo o seu modo de escrever, e conforme a sua língua.
                            Então foram chamados os escrivães do rei, naquele mesmo tempo, no terceiro mês (que é o mês de Sivã), aos vinte e três dias; e se escreveu conforme a tudo quanto ordenou Mardoqueu aos judeus, como também aos sátrapas, e aos governadores, e aos líderes das províncias, que se estendem da Úndia até Etiópia, cento e vinte e sete províncias, a cada província segundo o seu modo de escrever, e a cada povo conforme a sua língua; como também aos judeus segundo o seu modo de escrever, e conforme a sua língua.

                            Ester 8:9
                        </div>
                    </v-flex>
                    <v-flex md6 class="text-rotate">
                        SOBRE
                    </v-flex>
                </v-layout>
            </v-flex>
        </v-layout>
        <!-- terceira sessão -->
        <v-layout>
            <v-flex xs12 md3>
                <div class="contatos" v-wow="{ 'animation-name': 'fadeInRight','animation-duration': '1s'}">
                    <div class="box-1-bottom">
                        <div>Contatos</div>
                    </div>
                    <div class="box-2-bottom">
                        <div class="title">Brasília/DF</div>
                        <div class="subheading">SAUS Quadra 5 | Bloco N | Lote 2 | 10 º andar</div>
                        <div class="subheading">Tel: +55(61) 3208-1155</div>
                    </div>
                    <div class="space-md"></div>
                    <div class="box-3-bottom">
                        <div class="title">São Paulo/SP</div>
                        <div class="subheading">Rua Estados Unidos 367, Jardim Paulista</div>
                        <div class="subheading">Tel: +55(61) 2050-2410</div>
                    </div>
                    <div class="box-4-bottom">
                        <v-card-text>
                            <v-btn
                                    v-for="icon in icons"
                                    :key="icon"
                                    class=""
                                    icon
                            >
                                <v-icon size="24px" class="color-icon">{{ icon }}</v-icon>
                            </v-btn>
                        </v-card-text>
                    </div>
                </div>
            </v-flex>
            <v-flex xs12 md9>
                <div class="bg-img-3 right-triangle">

                </div>
            </v-flex>
            </div>
        </v-layout>
    </v-container>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      menu: [
        {name: 'sobre'},
        {name: 'serviços'},
        {name: 'portifólio'},
        {name: 'prêmios'},
        {name: 'clientes'},
        {name: 'contato'}
      ],
      icons: [
        'fab fa-facebook',
        'fab fa-twitter',
        'fab fa-google-plus',
        'fab fa-linkedin',
        'fab fa-instagram'
      ]
    }
  },
  components: {}
}
</script>
