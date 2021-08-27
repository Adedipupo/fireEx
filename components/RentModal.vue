<template>
  <div>
    <b-button id="show-btn" @click="showModal">Rent</b-button>

    <b-modal ref="my-modal" hide-footer title="Using Component Methods">
      <div class="calender-container">
        <div class="text-container">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus
            laboriosam aut dolorum quos adipisci porro eius iusto, reprehenderit
            totam ipsum omnis repellendus quia obcaecati aliquam? Rem repellat
            tenetur dolore eveniet?
          </p>
        </div>
      </div>
      <b-button id="show-btn" variant="outline-danger">Close</b-button>
    </b-modal>
  </div>
</template>

<script>
export default {
  methods: {
    showModal() {
      this.$refs["my-modal"].show();
    },
    hideModal() {
      this.$refs["my-modal"].hide();
    }
  }
};
</script>

<style scoped>
button {
  width: 100%;
  border: none;
  padding: 0.5rem;
  color: white;
  font-weight: 700;
  padding: 1rem 4rem;
  border-radius: 100rem;
  background-color: rgb(231, 81, 43);
  color: white;
  font-weight: 700;
  transition: 0.5s;
}
.calendar-container {
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}
p {
  color: grey;
}
.text-container {
  padding: 0.5rem;
}
</style>
