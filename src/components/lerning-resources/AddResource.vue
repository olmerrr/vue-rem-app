<template>
  <base-card>
    <form>
      <div class="form-controll">
        <label for="title">Title</label>
        <input id="title" name="title" type="text" />
      </div>

      <div class="form-controll">
        <label for="description">Description</label>
        <textarea id="description" name="description" rows="3"></textarea>
      </div>

      <div class="form-controll">
        <label for="link">Link</label>
        <input id="link" name="link" type="url" />
      </div>

      <div class="btn-form-sub">
        <base-button type="submit">Add Resurce</base-button>
      </div>
    </form>
  </base-card>
</template>

<script>
export default {};
</script>
<style scoped>
label {
  font-weight: bold;
  display: block;
  margin-bottom: 0.5rem;
}

input,
textarea {
  display: block;
  width: 100%;
  font: inherit;
  padding: 0.15rem;
  border: 1px solid #ccc;
}

input:focus,
textarea:focus {
  outline: none;
  border-color: #3a0061;
  background-color: #f7ebff;
}

.form-control {
  margin: 1rem 0;
}
.btn-form-sub{
  margin-top: 20px;
}
</style>