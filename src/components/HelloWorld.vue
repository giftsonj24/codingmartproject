<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <form>
      <table>
        <tr>
          <td>Employee Name</td>
          <td><input type="text" v-model="name" /></td>
        </tr>
        <tr>
          <td>Email</td>
          <td><input type="email" v-model="email" /></td>
        </tr>
      </table>
      <div class="div"><button class="button">Save</button></div>
    </form>
    <div class="hello">
      <form>
        <table>
          <tr>
            <td>Employee Name</td>
            <td><input type="text" v-model="name" /></td>
          </tr>
          <tr>
            <td>Date</td>
            <td><input type="text" v-model="date" /></td>
          </tr>
          <tr>
            <td>Attendance</td>
            <td>
              <select>
                <option value="Present">Present</option>
                <option value="Absent">Absent</option>
              </select>
            </td>
          </tr>
        </table>
        <div class="div"><button class="button">Save</button></div>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  border-style: solid;
  border-width: 1px;
  width: 800px;
  height: 240px;
  margin-top: 50px;
  margin-left: auto;
  margin-right: auto;
  padding: 7px;
}

table {
  padding: 5px;
}

input[type="text"],
input[type="email"],
select {
  background-color: lightgrey;
  width: 100%;
  padding: 10px;
  margin: 10px;
  border: 0;
}

.div {
  text-align: center;
}

.button {
  width: 6%;
}
</style>
