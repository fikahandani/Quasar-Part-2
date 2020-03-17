<template>
  <q-page>
    <q-card class="col-lg-12 col-xs-12 q-pa-lg">
      <q-card-title align="center">Form Registration</q-card-title>
      <q-card-main class="q-pa-sm">
        <div class="row items-end">
          <div class="col-xs-12 col-lg-12 q-pa-sm">
            <q-input required v-model="firstName" float-label="First Name" type="text" />
          </div>
          <div class="col-xs-12 col-lg-12 q-pa-sm">
            <q-input required v-model="lastName" float-label="Last Name" type="text" />
          </div>
          <div class="col-xs-12 col-lg-12 q-pa-sm">
            <q-input required v-model="address" float-label="Address" type="text" />
          </div>
          <div class="col-xs-12 col-lg-6 q-pa-sm">
          <q-select filter v-model="provinsi" :options="optionsProv" float-label="Provinsi" />
        </div>
        <div class="col-xs-12 col-lg-6 q-pa-sm">
          <q-select filter v-model="kota" :options="optionsKota" float-label="Kota" />
        </div>
        </div>
        <div align="right" class="q-mt-lg">
          <q-btn class="q-ma-sm" label="Cancel" icon="cancel" color="red" size="15px" />
          <q-btn class="q-ma-sm" label="Save" icon="save" color="secondary" size="15px"/>
        </div>
        
      </q-card-main>
      
    </q-card>
  </q-page>
</template>

<script>
export default {
  data() {
    return {
      firstName: "",
      lastName: "",
      address: "",
      provinsi: "",
      optionsProv: [
        {
          label: "Jawa Timur",
          value: "jawaTimur"
        },
        {
          label: "Jawa Tengah",
          value: "jawaTengah"
        },
        {
          label: "Jawa Barat",
          value: "jawaBarat"
        }
      ],
      kota: "",
      optionsKota: [
        {
          label: "Malang",
          value: "malang",
        },
        {
          label: "Batu",
          value: "batu",
        },
        {
          label: "Kediri",
          value: "kediri",
        },
        {
          label: "Solo",
          value: "solo",
        },
        {
          label: "Sragen",
          value: "sragen",
        },
        {
          label: "Blitar",
          value: "blitar",
        },
        {
          label: "Jakarta",
          value: "jakarta",
        },
        {
          label: "Bekasi",
          value: "bekasi",
        },
        {
          label: "Bogor",
          value: "bogor",
        },
        {
          label: "Tangerang",
          value: "tangerang",
        },
      ]

    };
  }
};
</script>
