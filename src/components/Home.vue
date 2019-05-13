<template>
  <div>
    {{ root_group }}
  </div>
</template>

<script>
  export default {
    name: 'Home',
    data() {
      return {
        root_group: {
          type: "group",
          name: "My tasks",
          items: [
            {
              type: "item",
              name: "Build a tree",
              done: false
            },
            {
              type: "group",
              name: "Interview",
              items: [
                {
                  type: "item",
                  name: "read docs",
                  done: true
                },
                {
                  type: "item",
                  name: "read docs once again",
                  done: true
                },
              ]
            }
          ]
        }
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h3 {
    margin: 40px 0 0;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
