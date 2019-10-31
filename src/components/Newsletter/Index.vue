<template>
  <div class="container newsl_container">
    <h2>Join our newsletter</h2>
    <div class="form">
      <input type="text" v-model="email" />
      <button @click="submitHandler">Subscribe</button>
    </div>
    <div class="error_label">
      <div>{{error}}</div>
    </div>
    <div class="success_label">
      <div>{{success}}</div>
    </div>
    <div class="small">
      <div>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet corrupti laboriosam necessitatibus quasi sapiente asperiores quod autem voluptas! Optio, sapiente.</div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      error: "",
      success: ""
    };
  },
  methods: {
    validate(email) {
      let valid = [true, ""];
      if (!/^([\w.-]+)@([\w-]+)((\.(\w){2,3})+)$/.test(email)) {
        valid = [false, "Enter a valid email"];
      }
      if (email === "") {
        valid = [false, "It's empty"];
      }
      return valid;
    },
    submitHandler() {
      let valid = this.validate(this.email);
      if (valid[0]) {
        this.error = "";
      } else {
        this.error = valid[1];
      }
    }
  }
};
</script>