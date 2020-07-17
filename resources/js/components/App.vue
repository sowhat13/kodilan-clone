<template>
  <div>
    <navbar></navbar>
    <card></card>
    <notices></notices>
  </div>
</template>

<script>
import Navbar from "./Navbar";
import Card from "./Card";
import Notices from "./Notices";

export default {
  components: { Navbar, Card, Notices }
};
</script>
