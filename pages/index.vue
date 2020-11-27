<template>
  <div>
    <header>
      <h1>Inputs</h1>
    </header>
    <main>
      <div class="main">
        <div class="lign">
          <div class="input-container">
            <p>< Input /></p>
            <label>Label</label>
            <b-form-input v-model="text" placeholder="Placeholder" class="input-classic"></b-form-input>
          </div>
          <div class="input-container">
            <p>< Input error /></p>
            <label>Label</label>
            <b-form-input :state="false" v-model="text" placeholder="Placeholder" class="input-error"></b-form-input>
          </div>
          <div class="input-container">
            <p>< Input disabled /></p>
            <label>Label</label>
            <b-form-input :disabled="true" v-model="text" placeholder="Placeholder"></b-form-input>
          </div>
        </div>
        <div class="lign">
          <div class="input-container">
            <p>< Input helperText="Some interesting text" /></p>
            <label>Label</label>
            <b-form-input v-model="text" placeholder="Placeholder" class="input-helperText"></b-form-input>
            <b-form-text>Some interesting text</b-form-text>
          </div>
          <div class="input-container">
            <p>< Input helperText="Some interesting text" error /></p>
            <label>Label</label>
            <b-form-input :state="false" v-model="text" placeholder="Placeholder" class="input-helperText"></b-form-input>
            <b-form-invalid-feedback>Some interesting text</b-form-invalid-feedback>
          </div>
        </div>
        <div class="lign">
          <div class="input-container">
            <p>< Input startIcon /></p>
            <label>Label</label>
            <b-input-group>
              <template #prepend>
                <b-input-group-text ><i class="material-icons">call</i></b-input-group-text>
              </template>
              <b-form-input v-model="text" placeholder="Placeholder"></b-form-input>
            </b-input-group>
          </div>
          <div class="input-container">
            <p>< Input endIcon /></p>
            <label>Label</label>
            <b-input-group>
              <b-form-input v-model="text" placeholder="Placeholder"></b-form-input>
              <template #append>
                <b-input-group-text ><i class="material-icons">lock</i></b-input-group-text>
              </template>
            </b-input-group>
          </div>
        </div>
        <div class="lign">
          <div class="input-container">
            <p>< Input value="text" /></p>
            <label>Label</label>
            <b-form-input v-model="inputText" value="text"></b-form-input>
          </div>
        </div>
        <div class="lign">
          <div class="input-container">
            <p>< Input size="sm" /></p>
            <label>Label</label>
            <b-form-input size="sm" v-model="text" placeholder="Placeholder"></b-form-input>
          </div>
          <div class="input-container">
            <p>< Input size="md" /></p>
            <label>Label</label>
            <b-form-input v-model="text" placeholder="Placeholder"></b-form-input>
          </div>
        </div>
        <div class="lign">
          <div class="input-container w-100">
            <p>< Input fullWidth /></p>
            <label>Label</label>
            <b-form-input size="10" v-model="text" placeholder="Placeholder"></b-form-input>
          </div>
        </div>
        <div class="lign">
          <div class="input-container">
            <p>< Input multiline row="4" /></p>
            <label>Label</label>
            <b-form-textarea
              placeholder="Placeholder"
              rows="4"
              no-resize
            ></b-form-textarea>
          </div>
        </div>
      </div>
    </main>
    <footer>
      <p>Alexandre Pouivet @DevChallenges.io</p>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      inputText: "Text",
    }
  }
}
</script>
