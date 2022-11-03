
      <template>


        <div>




          <v-card
              elevation="2"


          >
            <h3 class="pa-2">Подписки пользователья</h3>
            <v-divider></v-divider>
            <div class="d-flex flex-wrap">
              <v-chip v-for="item in userSubscriptions"
                      :key="item.id"

                      class="ma-2 "

                      color="primary"
              >
                {{item.name}}&nbsp;ID:&nbsp;{{item.id}}
              </v-chip>
            </div>
          </v-card>

        </div>
      </template>



<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      userSubscriptions: [
        {
          "id": 1,
          "layout_id": 2,
          "is_active": true,
          "name": "earum"
        },
        {
          "id": 4,
          "layout_id": 3,
          "is_active": true,
          "name": "abcdbv"
        },
      ],

    }),
  }
</script>
