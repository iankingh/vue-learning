<!-- 自製tableVue元件 -->
<template>
  <div>
    <table class="table table-striped">
      <thead>
        <tr>
          <th scope="col">ID</th>
          <th scope="col">Name</th>
          <th scope="col">Email</th>
          <th scope="col">Phone</th>
          <th scope="col">Address</th>
          <th scope="col">Action</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in items" :key="item.id">
          <td>{{ item.id }}</td>
          <td>{{ item.name }}</td>
          <td>{{ item.email }}</td>
          <td>{{ item.phone }}</td>
          <td>{{ item.address }}</td>
          <td>
            <button class="btn btn-primary" @click="edit(item)">Edit</button>
            <button class="btn btn-danger" @click="del(item)">Delete</button>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
<script>
export default {
    name: "tableVue",
    props: ["items"],
    methods: {
        edit(item) {
        this.$emit("edit", item);
        },
        del(item) {
        this.$emit("del", item);
        }
    }

    
}
</script>