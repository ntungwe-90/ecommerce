<template>
    <div>
        <Nav/>
      <Nuxt />
      <Footer/>
    </div>
  </template>
  
  <style>
  html {
    /* font-family: 'Nunito', 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
      Roboto, 'Helvetica Neue', Arial, sans-serif; */
    font-family: 'Nunito';
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }
  *,
  *::before,
  *::after {
    box-sizing: border-box;
    margin: 0;
  }
  .button--hero {
    display: inline-block;
    color: #fff;
    text-decoration: none;
    padding: 10px 30px;
  }
  .button--green {
    display: inline-block;
    border: 1px solid #3b8070;
    color: #3b8070;
    text-decoration: none;
    padding: 10px 30px;
  }
  .button--green:hover {
    color: #fff;
    background-color: #3b8070;
  }
  .button--grey {
    display: inline-block;
    border: 1px solid #35495e;
    color: #35495e;
    text-decoration: none;
    padding: 10px 30px;
    margin-left: 15px;
  }
  .button--grey:hover {
    color: #fff;
    background-color: #35495e;
  }
  .button--delete {
    display: inline-block;
    border: 1px solid #35495e;
    padding: 5px;
    color: white;
    background-color: #35495e;
  }
  button:focus {
    outline: none;
  }
  .container {
    width: 80%;
  }
  </style>