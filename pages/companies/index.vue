<template>
  <section class="py-[200px] flex flex-col items-center justify-center px-4">
    <div class="text-[32px] font-semibold text-dark mb-4">Select Companies</div>
    <div class="w-full card">
      <div class="form-group">
        <label for="" class="text-grey">Companies</label>

        <select name="" id=""
          class="appearance-none input-field form-icon-chevron_down">
          <option value="" selected>
            Company Name
          </option>
        </select>
        <!-- <p v-if="$fetchState.pending">Fetching companies...</p> -->
        <!-- <select v-else
          v-model="selectedCompany"
          name="companies"
          id=""
          class="appearance-none input-field form-icon-chevron_down"
        >
          <option :value="company.id" :key=company.id v-for="company in companies.data.result.data">
            {{ company.name }}
          </option>
        </select> -->
      </div>
      <a href="/companies/1" class="w-full btn btn-primary mt-[14px]">
        Continue
      </a>
    </div>
  </section>
</template>

<script>
export default {
  middleware: 'auth',
}
</script>