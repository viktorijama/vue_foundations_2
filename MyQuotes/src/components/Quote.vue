<template>
  <div class="col-ms-6 col-md-4 col-lg-3">
    <div class="panel panel-default">
      <div class="panel-body quote">
        <slot></slot>
        </div>
    </div>
  </div>
</template>

<style>
    .panel-body {
    font-family: 'Montserrat', sans-serif;
    font-size: 24px;
    color: #000000;
  }

  .quote {
    cursor: pointer;
  }

  .quote:hover {
    background-color: #d9edf7;
  }
</style>


