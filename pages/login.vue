<template>
    <div class="login">
      <h1>Login</h1>
      <form @submit.prevent="handleLogin">
        <input
          type="text"
          v-model="username"
          placeholder="Username"
          required
        />
        <input
          type="password"
          v-model="password"
          placeholder="Password"
          required
        />
        <button type="submit">Login</button>
      </form>
      <p v-if="errorMessage" class="error">{{ errorMessage }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Login',
    data() {
      return {
        username: '',
        password: '',
        errorMessage: '',
      };
    },
    methods: {
      handleLogin() {
        if (this.username === 'admin' && this.password === '12345') {
          alert('Login berhasil!');
          this.$router.push('/');
        } else {
          this.errorMessage = 'Username atau password salah!';
        }
      },
    },
  };
  </script>
  
  <style scoped>
  .login {
    width: 30%;
    margin: 50px auto;
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 5px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    font-family: Arial, sans-serif;
  }
  h1 {
    text-align: center;
  }
  form {
    display: flex;
    flex-direction: column;
  }
  input {
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  button {
    background-color: #007bff;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  button:hover {
    background-color: #0056b3;
  }
  .error {
    color: red;
    text-align: center;
  }
  </style>
  